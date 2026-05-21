export default function Portfolio() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-pink-50 to-white text-gray-800 font-sans">
      {/* NAVBAR */}
      <nav className="w-full flex justify-between items-center px-8 py-6 border-b border-pink-100 backdrop-blur-sm sticky top-0 bg-white/80 z-50">
        <h1 className="text-2xl font-bold text-pink-500">Marie Kasongo ✨</h1>

        <div className="hidden md:flex gap-8 text-sm font-medium text-pink-400">
          <a href="#about" className="hover:text-pink-600 transition">About</a>
          <a href="#research" className="hover:text-pink-600 transition">Research</a>
          <a href="#projects" className="hover:text-pink-600 transition">Projects</a>
          <a href="#skills" className="hover:text-pink-600 transition">Skills</a>
          <a href="#resume" className="hover:text-pink-600 transition">Resume</a>
          <a href="#contact" className="hover:text-pink-600 transition">Contact</a>
        </div>
      </nav>

      {/* HERO SECTION */}
      <section className="max-w-7xl mx-auto px-8 py-20 grid md:grid-cols-2 gap-16 items-center">
        <div>
          <p className="text-2xl mb-4">Hi, I’m</p>

          <h1 className="text-6xl md:text-7xl font-black text-pink-500 leading-tight mb-6">
            Marie Kasongo
          </h1>

          <h2 className="text-3xl font-semibold mb-6 leading-snug">
            Biomedical Engineering Student <br />
            at Brown University
          </h2>

          <p className="text-lg text-gray-600 leading-relaxed mb-10 max-w-xl">
            Passionate about biomedical imaging, cancer research, and using computational tools to solve real-world healthcare problems.
          </p>

          <div className="flex flex-wrap gap-4">
            <button className="bg-pink-500 hover:bg-pink-600 transition text-white px-8 py-4 rounded-2xl shadow-lg text-lg font-medium">
              View My Work ↓
            </button>

            <button className="border-2 border-pink-300 hover:border-pink-500 hover:text-pink-500 transition px-8 py-4 rounded-2xl text-lg font-medium text-pink-400 bg-white">
              Download Resume
            </button>
          </div>
        </div>

        <div className="flex justify-center">
          <div className="bg-pink-100 p-3 rounded-[40px] shadow-2xl shadow-pink-200/50">
            <img
              src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop"
              alt="Marie"
              className="w-[420px] h-[520px] object-cover rounded-[32px]"
            />
          </div>
        </div>
      </section>

      {/* DROPDOWN SECTIONS */}
      <section className="max-w-5xl mx-auto px-6 pb-24 space-y-8">

        {/* ABOUT */}
        <details id="about" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>💗 About Me</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8 text-lg leading-relaxed text-gray-600">
            I am a Biomedical Engineering student interested in biomedical imaging, AI in healthcare, computational biology, and translational medicine. My work combines engineering, research, and scientific problem solving to explore how technology can improve patient outcomes and healthcare innovation.
          </div>
        </details>

        {/* RESEARCH */}
        <details id="research" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>🧪 Research Experience</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8 text-lg text-gray-600 leading-relaxed space-y-4">
            <div>
              <h3 className="text-2xl font-semibold text-gray-800 mb-2">Wong Biomedical Imaging Lab</h3>
              <p>
                Conducting research involving circulating tumor cell morphology analysis using CellProfiler, Cellpose, PCA analysis, and fluorescence imaging workflows.
              </p>
            </div>

            <div>
              <h3 className="text-2xl font-semibold text-gray-800 mb-2">Research Interests</h3>
              <ul className="list-disc ml-6 space-y-2">
                <li>Biomedical imaging</li>
                <li>Cancer research</li>
                <li>Computational biology</li>
                <li>AI in healthcare</li>
              </ul>
            </div>
          </div>
        </details>

        {/* PROJECTS */}
        <details id="projects" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>💻 Featured Projects</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8 grid md:grid-cols-2 gap-6">
            <div className="bg-pink-50 rounded-2xl p-6 border border-pink-100">
              <h3 className="text-2xl font-bold text-pink-500 mb-3">CTC Morphology Analysis</h3>
              <p className="text-gray-600 leading-relaxed">
                Research project investigating how extracellular matrix stiffness affects circulating tumor cell morphology using computational imaging analysis.
              </p>
            </div>

            <div className="bg-pink-50 rounded-2xl p-6 border border-pink-100">
              <h3 className="text-2xl font-bold text-pink-500 mb-3">MATLAB Mass Launcher</h3>
              <p className="text-gray-600 leading-relaxed">
                Engineering simulation project involving ODE solving, projectile modeling, and launch velocity analysis.
              </p>
            </div>
          </div>
        </details>

        {/* SKILLS */}
        <details id="skills" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>✨ Technical Skills</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8 grid md:grid-cols-2 gap-8">
            <div>
              <h3 className="text-2xl font-bold text-gray-800 mb-4">Programming</h3>
              <div className="flex flex-wrap gap-3">
                {['Python', 'MATLAB', 'Data Visualization'].map((skill) => (
                  <span key={skill} className="bg-pink-100 text-pink-600 px-4 py-2 rounded-full font-medium">
                    {skill}
                  </span>
                ))}
              </div>
            </div>

            <div>
              <h3 className="text-2xl font-bold text-gray-800 mb-4">Research Tools</h3>
              <div className="flex flex-wrap gap-3">
                {['CellProfiler', 'Cellpose', 'Microscopy Analysis', 'PCA Analysis'].map((skill) => (
                  <span key={skill} className="bg-pink-100 text-pink-600 px-4 py-2 rounded-full font-medium">
                    {skill}
                  </span>
                ))}
              </div>
            </div>
          </div>
        </details>

        {/* RESUME */}
        <details id="resume" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>📄 Resume</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8">
            <button className="bg-pink-500 hover:bg-pink-600 transition text-white px-8 py-4 rounded-2xl shadow-lg text-lg font-medium">
              Download Resume
            </button>
          </div>
        </details>

        {/* CONTACT */}
        <details id="contact" className="group bg-white rounded-3xl border border-pink-100 shadow-sm overflow-hidden">
          <summary className="flex justify-between items-center cursor-pointer px-8 py-7 text-3xl font-bold text-pink-500 list-none">
            <span>💌 Contact</span>
            <span className="group-open:rotate-180 transition">⌄</span>
          </summary>

          <div className="px-8 pb-8 text-lg text-gray-600 space-y-3">
            <p>Email: marie@example.com</p>
            <p>LinkedIn: coming soon</p>
            <p>GitHub: marie-kasongo</p>
          </div>
        </details>
      </section>

      {/* FOOTER */}
      <footer className="border-t border-pink-100 py-10 text-center text-gray-500 text-sm">
        © 2026 Marie Kasongo • Built with 💗 and GitHub Pages
      </footer>
    </div>
  )
}

