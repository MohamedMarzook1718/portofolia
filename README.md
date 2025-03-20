import React from 'react';
import { motion } from 'framer-motion';

const App = () => {
  return (
    <div className="bg-black text-white min-h-screen">
      {/* Header Section */}
      <header className="p-6 flex justify-between items-center">
        <h1 className="text-3xl font-bold text-yellow-400">Mohamed Marzook E.S</h1>
        <a href="#contact" className="bg-yellow-400 text-black px-4 py-2 rounded-lg hover:bg-yellow-300 transition">Contact</a>
      </header>

      {/* Hero Section */}
      <section className="flex flex-col items-center justify-center h-screen text-center">
        <motion.h2 
          className="text-5xl font-extrabold text-yellow-400"
          initial={{ opacity: 0, y: -20 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
        >
          Hi, I'm Mohamed!
        </motion.h2>
        <p className="mt-4 text-lg text-gray-300">Web Developer & Video Editor | Passionate about coding and creativity.</p>
        <a href="#about" className="mt-6 bg-yellow-400 text-black px-6 py-3 rounded-lg hover:bg-yellow-300 transition">Learn More</a>
      </section>

      {/* About Me Section */}
      <section id="about" className="p-10">
        <h3 className="text-3xl text-yellow-400 font-bold">About Me</h3>
        <p className="mt-4 text-gray-300">
          I'm a Computer Science graduate from Bharathiar University (2023 - 2026), specializing in Python, JavaScript, and web technologies.
          I also excel in video editing using Premiere Pro, After Effects, and DaVinci Resolve.
        </p>
      </section>

      {/* Skills Section */}
      <section id="skills" className="p-10 bg-gray-900">
        <h3 className="text-3xl text-yellow-400 font-bold">Skills</h3>
        <div className="grid grid-cols-2 gap-4 mt-4">
          <span className="bg-gray-800 p-4 rounded-lg text-center">Python</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">JavaScript</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">C / C++</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">HTML & CSS</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">Premiere Pro</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">After Effects</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">DaVinci Resolve</span>
          <span className="bg-gray-800 p-4 rounded-lg text-center">Photoshop</span>
        </div>
      </section>

      {/* Achievements Section */}
      <section id="achievements" className="p-10">
        <h3 className="text-3xl text-yellow-400 font-bold">Achievements</h3>
        <ul className="mt-4 text-gray-300 list-disc pl-5">
          <li>1st Prize in Reels Making Competition</li>
          <li>Multiple Awards in Short Film Making Competitions</li>
        </ul>
      </section>

      {/* Contact Section */}
      <section id="contact" className="p-10 bg-gray-900">
        <h3 className="text-3xl text-yellow-400 font-bold">Contact</h3>
        <p className="mt-4 text-gray-300">Feel free to reach out via email:</p>
        <a href="mailto:mohamedmarzookes23cse@vetias.ac.in" className="mt-2 block text-yellow-400 hover:underline">
          mohamedmarzookes23cse@vetias.ac.in
        </a>
      </section>

      {/* Footer */}
      <footer className="p-4 text-center text-gray-500 bg-black">
        © 2025 Mohamed Marzook E.S. All Rights Reserved.
      </footer>
    </div>
  );
};

export default App;

