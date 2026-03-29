# Man_ma
Manma creates the development…


<html>
<head>
    <title>My Website</title>
</head>
<body>
    <h1>Welcome to My Official Site!</h1>
    

import React from 'react';
import { Layout, BarChart3, Globe, ShieldCheck, ArrowRight } from 'lucide-react';

const LandingPage = () => {
  return (
    <div className="min-h-screen bg-slate-50 font-sans text-slate-900">
      {/* Navigation / Index */}
      <nav className="sticky top-0 z-50 flex items-center justify-between px-8 py-4 bg-white/80 backdrop-blur-md border-b border-slate-200">
        <div className="text-2xl font-bold tracking-tighter text-blue-600">CORE.inc</div>
        <ul className="hidden md:flex space-x-8 font-medium text-slate-600">
          <li className="hover:text-blue-600 cursor-pointer transition">Solutions</li>
          <li className="hover:text-blue-600 cursor-pointer transition">Architecture</li>
          <li className="hover:text-blue-600 cursor-pointer transition">Analytics</li>
          <li className="hover:text-blue-600 cursor-pointer transition">Contact</li>
        </ul>
        <button className="bg-slate-900 text-white px-5 py-2 rounded-full font-medium hover:bg-slate-800 transition">
          Get Started
        </button>
      </nav>

      {/* Hero Section with Business Image Background */}
      <header className="relative h-[80vh] flex items-center justify-center overflow-hidden">
        <img 
          src="https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&q=80&w=2000" 
          alt="Modern Office" 
          className="absolute inset-0 w-full h-full object-cover"
        />
        <div className="absolute inset-0 bg-slate-900/60" /> {/* Dark Overlay for Text Clarity */}
        
        <div className="relative z-10 text-center px-4">
          <h1 className="text-5xl md:text-7xl font-extrabold text-white mb-6 tracking-tight">
            Scale Your <span className="text-blue-400">Digital Assets.</span>
          </h1>
          <p className="text-lg md:text-xl text-slate-200 max-w-2xl mx-auto mb-8 font-light">
            Integrated business systems designed for the modern enterprise. 
            Clean code, robust security, and real-time scalability.
          </p>
          <div className="flex flex-col sm:flex-row justify-center gap-4">
            <button className="flex items-center justify-center gap-2 bg-blue-600 text-white px-8 py-4 rounded-lg font-semibold hover:bg-blue-500 transition">
              View Repository <ArrowRight size={20} />
            </button>
            <button className="bg-white/10 backdrop-blur-sm border border-white/30 text-white px-8 py-4 rounded-lg font-semibold hover:bg-white/20 transition">
              Documentation
            </button>
          </div>



