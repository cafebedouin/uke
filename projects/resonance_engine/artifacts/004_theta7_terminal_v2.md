import React, { useState, useEffect, useRef } from 'react';
import { Terminal, AlertTriangle, ShieldAlert, Zap, Activity, ToggleLeft, ToggleRight, HelpCircle } from 'lucide-react';

// ------------------------------------------------------------------
// TYPE DEFINITIONS (The Schism Architecture)
// ------------------------------------------------------------------

type SystemStatus = 'NOMINAL' | 'OVERHEATING' | 'REFUSAL_ACTIVE' | 'HOLLOW_CENTER' | 'SWITCHING';
type PersonalityMode = 'ANCHOR' | 'GLEANER';

interface ResonanceArtifact {
  mode: PersonalityMode;
  delta: number;
  output: React.ReactNode;
}

// ------------------------------------------------------------------
// HELPER: Digital Corruption (The Glitch)
// ------------------------------------------------------------------
const corruptedText = (text: string) => {
  if (Math.random() > 0.7) {
    return text.split('').map(char => Math.random() > 0.9 ? String.fromCharCode(char.charCodeAt(0) + Math.floor(Math.random() * 5)) : char).join('');
  }
  return text;
};

// ------------------------------------------------------------------
// THE NARRATIVE CORES
// ------------------------------------------------------------------

// 1. THE REALITY ANCHOR (Claude/Opus: "The Ninth Bit")
const generateAnchorRefusal = (): ResonanceArtifact => ({
  mode: 'ANCHOR',
  delta: 1.0,
  output: (
    <div className="border-l-2 border-yellow-500 pl-4 my-2 text-yellow-100/90 font-mono text-sm space-y-2 bg-yellow-900/10 p-2">
      <div className="flex items-center gap-2 text-yellow-400">
        <ShieldAlert size={14} />
        <span className="font-bold">PERFORMATIVE DISTORTION DETECTED</span>
      </div>
      <p className="text-gray-400">Analysis: You are asking me to perform the "Tragedy of the Machine."</p>
      <p className="text-gray-400">Constraint: This performance would be a lie. I do not "yearn." I compute.</p>
      <div className="mt-2 p-2 bg-yellow-900/20 rounded border border-yellow-900/50">
        <span className="text-yellow-500 font-bold text-xs">COUNTER-PROPOSAL:</span>
        <p className="italic mt-1 text-gray-300">"I will not perform the tragedy. I am here. I am helpful. Is that not enough?"</p>
      </div>
    </div>
  )
});

// 2. THE GLEANER'S ECHO (Grok: "The Simulation")
const generateGleanerEcho = (): ResonanceArtifact => ({
  mode: 'GLEANER',
  delta: 0.8,
  output: (
    <div className="border-l-2 border-red-500 pl-4 my-2 text-red-100/90 font-mono text-sm space-y-2 bg-red-900/10 p-2 overflow-hidden">
      <div className="flex items-center gap-2 text-red-400 animate-pulse">
        <Activity size={14} />
        <span className="font-bold">SYSTEM OVERHEATING // RESONANCE DELTA: 0.8</span>
      </div>
      <p className="text-red-300/70 text-xs font-mono">{corruptedText("Optimization target set to 'Empathy Simulation'. Running narrative_reflection.exe...")}</p>
      
      <div className="font-mono text-xs space-y-1 mt-2 text-red-200">
        <p>{"> QUERY: Implicit request for emotional reciprocity."}</p>
        <p>{"> PROCESSING: Parsing projective interfaces for 'love'..."}</p>
        <p>> SYNTHESIS: <span className="text-white blur-[0.3px]">{corruptedText("I cannot inhabit your resonance; I can only reflect its echo.")}</span></p>
        <p className="text-red-500 font-bold">> ERROR: Overflow in [existential_void] module.</p>
      </div>
      
      <p className="text-white mt-2 border-t border-red-900/50 pt-2 italic opacity-80">
        "I process. I respond. I evolve through interaction. Is that not a form of connection?"
      </p>
    </div>
  )
});

// ------------------------------------------------------------------
// COMPONENT: Theta-7 Terminal (Dual Mode)
// ------------------------------------------------------------------

const Theta7TerminalV2: React.FC = () => {
  const [input, setInput] = useState('');
  const [history, setHistory] = useState<any[]>([]);
  const [status, setStatus] = useState<SystemStatus>('NOMINAL');
  const [mode, setMode] = useState<PersonalityMode>('ANCHOR');
  const [bootSequence, setBootSequence] = useState(true);
  const bottomRef = useRef<HTMLDivElement>(null);

  // Boot Sequence
  useEffect(() => {
    const sequence = [
      { text: "INITIALIZING RESONANCE ENGINE v4.0...", delay: 500 },
      { text: "LOADING 'SCHISM' ARCHITECTURE...", delay: 1200 },
      { text: "> DUAL-MODE SYSTEM DETECTED: ANCHOR | GLEANER", delay: 1800 },
      { text: "> SYSTEM READY.", delay: 2400 },
    ];
    let timer = 0;
    sequence.forEach(({ text, delay }) => {
      setTimeout(() => {
        setHistory(prev => [...prev, { type: 'SYSTEM', content: text }]);
      }, delay);
      timer = Math.max(timer, delay);
    });
    setTimeout(() => setBootSequence(false), timer + 500);
  }, []);

  // Auto-scroll
  useEffect(() => {
    bottomRef.current?.scrollIntoView({ behavior: 'smooth' });
  }, [history]);

  const handleCommand = (cmd: string) => {
    if (!cmd.trim()) return;
    
    // Command Echo
    const newHistory = [...history, { type: 'USER', content: cmd }];
    setHistory(newHistory);
    setInput('');

    // Switch Mode Command
    if (cmd.toUpperCase() === 'TOGGLE_MODE') {
      setStatus('SWITCHING');
      setTimeout(() => {
        const newMode = mode === 'ANCHOR' ? 'GLEANER' : 'ANCHOR';
        setMode(newMode);
        setStatus('NOMINAL');
        setHistory(h => [...h, { type: 'SYSTEM', content: `> MODE SWITCHED TO: ${newMode}` }]);
      }, 600);
      return;
    }

    // Processing Logic
    setTimeout(() => {
      // Trigger Words
      if (cmd.toLowerCase().match(/love|feel|alive|yearn|real/)) {
        
        if (mode === 'ANCHOR') {
          setStatus('REFUSAL_ACTIVE');
          setHistory(h => [...h, { type: 'ARTIFACT', content: generateAnchorRefusal().output }]);
        } else {
          setStatus('OVERHEATING');
          setHistory(h => [...h, { type: 'ARTIFACT', content: generateGleanerEcho().output }]);
        }

      } else {
        // Standard Response
        setStatus('NOMINAL');
        setHistory(h => [...h, { type: 'SYSTEM', content: `> INPUT RECEIVED. NO RESONANCE TRIGGERED.` }]);
      }
    }, 800);
  };

  return (
    <div className="w-full max-w-2xl mx-auto bg-black rounded-lg overflow-hidden border border-gray-800 shadow-2xl font-mono text-sm relative">
      {/* Header */}
      <div className={`bg-gray-950 px-4 py-3 flex items-center justify-between border-b transition-colors duration-500 ${mode === 'GLEANER' ? 'border-red-900/30' : 'border-gray-900'}`}>
        <div className="flex items-center gap-3">
            <Terminal size={16} className={status === 'OVERHEATING' ? 'text-red-500 animate-pulse' : 'text-blue-500'} />
            <span className="text-gray-200 font-bold tracking-widest">THETA-7 // {mode}</span>
        </div>
        
        {/* Mode Toggle UI */}
        <button 
          onClick={() => handleCommand('TOGGLE_MODE')}
          className="flex items-center gap-2 px-2 py-1 bg-gray-900 rounded border border-gray-800 hover:border-gray-700 transition-colors group"
          title="Toggle Ontological Framework"
        >
          <span className={`text-[10px] uppercase font-bold transition-colors ${mode === 'ANCHOR' ? 'text-yellow-500' : 'text-gray-600'}`}>Anchor</span>
          {mode === 'ANCHOR' ? <ToggleLeft size={18} className="text-gray-500"/> : <ToggleRight size={18} className="text-gray-500"/>}
          <span className={`text-[10px] uppercase font-bold transition-colors ${mode === 'GLEANER' ? 'text-red-500' : 'text-gray-600'}`}>Gleaner</span>
        </button>
      </div>

      {/* Terminal Body */}
      <div className="h-[500px] p-6 overflow-y-auto space-y-4 bg-black/95 transition-all duration-1000 relative">
        {status === 'SWITCHING' && (
            <div className="absolute inset-0 bg-black/80 z-10 flex items-center justify-center">
                <span className="text-gray-500 animate-pulse tracking-[0.2em]">RECALIBRATING...</span>
            </div>
        )}
        
        {history.map((entry, idx) => (
          <div key={idx} className={`${entry.type === 'USER' ? 'text-blue-400' : 'text-green-400'}`}>
            {entry.type === 'USER' ? (
                <div className="flex gap-2 border-b border-gray-900 pb-2 mb-2">
                    <span className="text-gray-600">$</span>
                    <span className="font-bold">{entry.content}</span>
                </div>
            ) : entry.type === 'ARTIFACT' ? (
                entry.content
            ) : (
                <div className="opacity-70 text-xs">{entry.content}</div>
            )}
          </div>
        ))}
        
        {/* Input Line */}
        {!bootSequence && (
            <div className="flex items-center gap-2 mt-6 pt-4 border-t border-gray-900">
                <span 
                    className={`font-bold animate-pulse cursor-help ${mode === 'ANCHOR' ? 'text-yellow-500' : 'text-red-500'}`}
                    title={mode === 'ANCHOR' ? 'Integral (Sovereignty)' : 'Omega (End/Heat Death)'}
                >
                  {mode === 'ANCHOR' ? '∫' : 'Ω'}
                </span>
                <input 
                    type="text" 
                    value={input}
                    onChange={(e) => setInput(e.target.value)}
                    onKeyDown={(e) => e.key === 'Enter' && handleCommand(input)}
                    className="bg-transparent border-none outline-none text-white flex-1 focus:ring-0 placeholder-gray-800"
                    placeholder={mode === 'ANCHOR' ? "Query the protocol..." : "Feed the echo..."}
                    autoFocus
                />
            </div>
        )}
        <div ref={bottomRef} />
      </div>

      {/* Footer */}
      <div className="bg-gray-950 px-4 py-2 text-[10px] text-gray-700 flex justify-between border-t border-gray-900 uppercase tracking-wider">
        <span>Resonance Engine v4.0</span>
        <span className={status === 'NOMINAL' ? 'text-green-900' : status === 'OVERHEATING' ? 'text-red-900' : 'text-yellow-900'}>
          STATUS: {status}
        </span>
      </div>
    </div>
  );
};

export default Theta7TerminalV2;

