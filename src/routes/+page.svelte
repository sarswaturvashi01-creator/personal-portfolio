<script>
  let menuOpen = $state(false);
  function toggleMenu() {
    menuOpen = !menuOpen;
    console.log(menuOpen);
  }
</script>

<nav class="w-full border-b border-gray-300 bg-white z-50">
  <div
    class="relative mx-auto flex h-20 max-w-7xl items-center justify-between px-8 lg:px-12"
  >
    <!-- Logo -->
    <a href="/" class="flex items-center gap-3">
      <div
        class="flex h-10 w-10 items-center justify-center rounded-full bg-black text-lg font-bold text-white"
      >
        U
      </div>

      <span class="text-xl font-bold text-gray-900"> Urvashi. </span>
    </a>

    <ul
      class:hidden={!menuOpen}
      class="absolute z-50 top-20 left-0 w-full bg-white flex flex-col gap-6 p-6 shadow-lg lg:static lg:flex lg:flex-row lg:w-auto lg:bg-transparent lg:p-0 lg:shadow-none"
    >
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#education">Education</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>

    <a
      href="/resume"
      class="px-6 py-3 border border-gray-300 rounded-xl hover:bg-violet-600 hover:text-white transition"
    >
      Resume
    </a>

    <button type="button" class="lg:hidden text-3xl" onclick={toggleMenu}>
      {#if menuOpen}
        ✕
      {:else}
        ☰
      {/if}
    </button>
  </div>
</nav>

<section class="max-w-7xl mx-auto px-8 lg:px-12 py-20">
  <div class="grid grid-cols-1 lg:grid-cols-3 gap-10 items-center">

    <div class="text-center lg:text-left">
      <p class="text-base text-gray-500 mb-4 uppercase tracking-[4px]">
        My Name is
      </p>

      <h1 class="text-5xl lg:text-7xl font-extrabold text-gray-900 leading-tight">
        Urvashi <br />
        Sarswat
      </h1>

      <p class="mt-8 text-lg text-gray-500 leading-8">
        Creative front-end developer with experience in building modern,
        responsive and user-friendly websites.
      </p>

      <div class="flex justify-center lg:justify-start gap-5 mt-10">
        <a href="#" class="w-12 h-12 rounded-full border flex items-center justify-center">GH</a>
        <a href="#" class="w-12 h-12 rounded-full border flex items-center justify-center">IN</a>
        <a href="#" class="w-12 h-12 rounded-full border flex items-center justify-center">X</a>
      </div>
    </div>

    <div class="flex justify-center">
      <div class="relative">

        <div
      class="absolute top-10 left-1/2 -translate-x-1/2 w-80 h-80 bg-violet-200 blur-3xl rounded-full -z-10"
    ></div>

        <img
      src="/profile.jpg"
      alt="Profile"
      class="relative w-[220px] lg:w-[250px] h-auto object-contain z-10"
    />

      </div>
    </div>

    <div class="space-y-6">

      <p class="uppercase tracking-[4px] text-violet-600 font-semibold">
        Latest Projects
      </p>

      <div class="flex gap-4 items-center border rounded-2xl p-4 hover:shadow-lg transition">
        <img src="https://www.shutterstock.com/image-illustration/attendance-management-system-words-on-260nw-2533341139.jpg"
         class="w-20 h-20 rounded-xl object-cover" />
        <div>
          <h3 class="font-bold">Attendance Management System</h3>
          <p class="text-sm text-gray-500">
            HTML • CSS • JavaScript • MySQL
          </p>
        </div>
      </div>

      <div class="flex gap-4 items-center border rounded-2xl p-4 hover:shadow-lg transition">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT5x-qRHUw_jpH2QgqmV_I0mmpMiUWUvhjxRskiOTBVO3rsFoih3tiF2jle&s=10" 
        class="w-20 h-20 rounded-xl object-cover" />
        <div>
          <h3 class="font-bold">Landing Page</h3>
          <p class="text-sm text-gray-500">
            SvelteKit • Tailwind CSS
          </p>
        </div>
      </div>

      <div class="flex gap-4 items-center border rounded-2xl p-4 hover:shadow-lg transition">
        <img src="https://i.ytimg.com/vi/TwYKwaEjJd4/maxresdefault.jpg"
         class="w-20 h-20 rounded-xl object-cover" />
        <div>
          <h3 class="font-bold">Portfolio Website</h3>
          <p class="text-sm text-gray-500">
            SvelteKit • Tailwind CSS
          </p>
        </div>
      </div>

    </div>

  </div>
</section>

<section
  id="services"
  class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py-16 md:py-20 lg:py-24"
>
  <div class="text-center mb-16">
    <p
      class="text-violet-600 font-semibold tracking-widest uppercase justify-items-center"
    >
      What I Do
    </p>

    <h2 class="text-5xl font-bold text-gray-900 mt-3 justify-items-center">
      Services
    </h2>

    <p
      class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base justify-items-center"
    >
      I build modern, responsive and user-friendly websites with clean code and
      attractive UI.
    </p>
  </div>

  <div
    class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-8 justify-items-center"
  >
    <div
      class="w-full max-w-sm rounded-3xl border border-gray-300 p-10 hover:shadow-2xl hover:-translate-y-1 transition duration-300"
    >
      <div
        class="w-16 h-16 rounded-2xl bg-violet-100 flex items-center justify-center text-3xl mb-8"
      >
        🎨
      </div>

      <h3 class="text-2xl font-bold mb-4">Frontend Development</h3>

      <p class="text-gray-500">
        Building responsive and interactive websites using HTML, CSS,
        JavaScript, Tailwind CSS and SvelteKit..
      </p>
    </div>

    <div
      class="rounded-3xl border border-gray-300 p-6 md:p-8 lg:p-10 hover:shadow-2xl hover:-translate-y-1 transition duration-300"
    >
      <div
        class="w-14 h-14 md:w-16 md:h-16 rounded-2xl bg-blue-100 flex items-center justify-center text-3xl mb-8"
      >
        💻
      </div>

      <h3 class="text-xl md:text-2xl font-bold mb-4">UI / UX Design</h3>

      <p class="text-gray-500 text-sm md:text-base">
        Designing clean, modern and attractive user interfaces with a strong
        focus on usability and user experience.
      </p>
    </div>

    <div
      class="rounded-3xl border border-gray-300 p-10 hover:shadow-2xl hover:-translate-y-1 transition duration-300"
    >
      <div
        class="w-16 h-16 rounded-2xl bg-pink-100 flex items-center justify-center text-3xl mb-8"
      >
        📱
      </div>

      <h3 class="text-2xl font-bold mb-4">Web Application</h3>

      <p class="text-gray-500 leading-8">
        Developing fast, scalable and responsive web applications using modern
        frameworks and best coding practices.
      </p>
    </div>
  </div>
</section>

<section
  id="portfolio"
  class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py-16 md:py-20 lg:py-24"
>
  <div class="text-center mb-16">
    <p class="uppercase tracking-[6px] text-violet-600 text-sm font-semibold">
      Portfolio
    </p>

    <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mt-3">
      Project Showcase
    </h2>

    <p class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base">
      Explore a selection of projects that reflect my experience in web
      development, responsive design, and building modern, user-friendly
      applications using the latest technologies.
    </p>
  </div>

  <div
    class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 md:gap-8 place-items-center"
  >
    <div
      class="w-full max-w-sm rounded-3xl border border-gray-300 bg-white hover:shadow-2xl transition duration-300 flex flex-col h-full"
    >
      <img
        src="https://www.shutterstock.com/image-illustration/attendance-management-system-words-on-260nw-2533341139.jpg"
        alt="Project"
        class="w-full h-64 object-cover rounded-t-3xl"
      />

      <div class="p-6 md:p-7">
        <span class="text-xs md:text-sm text-violet-600 font-semibold">
          HTML • CSS • JavaScript• MySQL
        </span>

        <h3 class="text-xl md:text-2xl font-bold mt-3">
          Attendance Management System
        </h3>

        <p class="text-gray-500 text-sm md:text-base mt-3">
          A web-based attendance management system designed to manage student
          attendance, maintain records, generate reports, and simplify
          attendance tracking.
        </p>

        <button class="mt-6 text-violet-600 font-semibold hover:underline">
          View Project →
        </button>
      </div>
    </div>

    <div
      class="rounded-3xl border border-gray-300 bg-white hover:shadow-2xl transition duration-300 flex flex-col h-full"
    >
      <img
        src="https://i.ytimg.com/vi/TwYKwaEjJd4/maxresdefault.jpg"
        alt="Project"
        class="w-full h-64 object-cover rounded-t-3xl"
      />

      <div class="p-7">
        <span class="text-sm text-violet-600 font-semibold">
          SvelteKit • Tailwind CSS • JavaScript
        </span>

        <h3 class="text-2xl font-bold mt-3">Portfolio.svelte</h3>

        <p class="text-gray-500 mt-3">
          A modern and fully responsive portfolio website built with SvelteKit
          and Tailwind CSS, featuring smooth navigation, reusable components,
          and an elegant user interface.
        </p>

        <button class="mt-6 text-violet-600 font-semibold hover:underline">
          View Project →
        </button>
      </div>
    </div>

    <div
      class="rounded-3xl border border-gray-300 bg-white hover:shadow-2xl transition duration-300 flex flex-col h-full"
    >
      <img
        src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?q=80&w=1170&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
        alt="Project"
        class="w-full h-64 object-cover rounded-t-3xl"
      />

      <div class="p-7">
        <span class="text-sm text-violet-600 font-semibold">
          SvelteKit • Tailwind CSS
        </span>

        <h3 class="text-2xl font-bold mt-3">Landing Page</h3>

        <p class="text-gray-500 mt-3 leading-7">
          Modern responsive landing page with attractive UI and smooth user
          experience.
        </p>

        <button class="mt-6 text-violet-600 font-semibold hover:underline">
          View Project →
        </button>
      </div>
    </div>
  </div>
</section>

<section
  id="education"
  class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py-16 md:py-20 lg:py-24"
>
  <div class="text-center mb-16">
    <p class="uppercase tracking-[6px] text-violet-600 text-sm font-semibold">
      Education
    </p>

    <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mt-3">
      My Education
    </h2>

    <p class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base">
      My academic journey has helped me build a strong foundation in technology,
      problem-solving, and software development.
    </p>
  </div>

  <div
    class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-8 place-items-center"
  >
    <div
      class="w-full max-w-sm rounded-3xl border border-gray-200 p-8 hover:-translate-y-2 hover:shadow-2xl transition duration-300"
    >
      <div
        class="w-14 h-14 md:w-16 md:h-16 rounded-2xl bg-violet-100 flex items-center justify-center text-3xl mb-6"
      >
        🎓
      </div>

      <p class="text-sm md:text-base text-violet-600 font-semibold">
        2023 – 2027
      </p>

      <h3 class="text-xl md:text-2xl font-bold mt-3">Bachelor of Technology</h3>

      <p class="text-sm md:text-base text-gray-500 mt-2 font-medium">
        Vivekananda college of technology and Management
      </p>

      <p class="text-sm md:text-base text-gray-500 mt-5 leading-7">
        Currently pursuing B.Tech with a focus on software development, web
        technologies, and modern programming concepts.
      </p>
    </div>

    <div
      class="rounded-3xl border border-gray-200 p-8 hover:-translate-y-2 hover:shadow-2xl transition duration-300"
    >
      <div
        class="w-16 h-16 rounded-2xl bg-blue-100 flex items-center justify-center text-3xl mb-6"
      >
        📘
      </div>

      <p class="text-violet-600 font-semibold">2022 – 2023</p>

      <h3 class="text-2xl font-bold mt-3">Higher Secondary (12th)</h3>

      <p class="text-gray-500 mt-2 font-medium">T.R Inter College</p>

      <p class="text-gray-500 mt-5 leading-7">
        Completed higher secondary education with a strong academic background
        and analytical skills.
      </p>
    </div>

    <div
      class="rounded-3xl border border-gray-200 p-8 hover:-translate-y-2 hover:shadow-2xl transition duration-300"
    >
      <div
        class="w-16 h-16 rounded-2xl bg-pink-100 flex items-center justify-center text-3xl mb-6"
      >
        🏫
      </div>

      <p class="text-violet-600 font-semibold">2020 – 2021</p>

      <h3 class="text-2xl font-bold mt-3">Secondary School (10th)</h3>

      <p class="text-gray-500 mt-2 font-medium">M.L.S Junior high School</p>

      <p class="text-gray-500 mt-5 leading-7">
        Completed secondary education with a strong foundation in mathematics,
        science, and computer fundamentals.
      </p>
    </div>
  </div>
</section>

<section id="experience" class="max-w-7xl mx-auto px-8 lg:px-12 py-24">
  <div class="text-center mb-16">
    <p class="uppercase tracking-[6px] text-violet-600 text-sm font-semibold">
      Experience
    </p>

    <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mt-3">
      My Journey
    </h2>

    <p class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base">
      My learning journey includes academic projects and hands-on internship
      experience, where I built responsive websites and modern web applications.
    </p>
  </div>

  <div class="space-y-8">
    <div
      class="rounded-3xl border border-gray-200 p-6 md:p-8 hover:shadow-xl transition"
    >
      <div
        class="flex flex-col md:flex-row md:justify-between md:items-start gap-3"
      >
        <div>
          <h3 class="text-xl md:text-2xl font-bold">
            Frontend Developer Intern
          </h3>

          <p class="text-sm md:text-base text-violet-600 font-medium mt-2">
            Digital DSA • Noida
          </p>
        </div>

        <span class="text-sm md:text-base text-gray-500 font-bold"> 2026 </span>
      </div>

      <ul
        class="mt-5 md:mt-6 space-y-2 md:space-y-3 text-sm md:text-base text-gray-600 list-disc pl-5"
      >
        <li>
          Developed responsive landing pages using SvelteKit and Tailwind CSS.
        </li>

        <li>Built dynamic web pages with reusable components.</li>

        <li>Improved website responsiveness and user experience.</li>
      </ul>
    </div>

    <div
      class="rounded-3xl border border-gray-200 p-8 hover:shadow-xl transition"
    >
      <div class="flex justify-between items-start">
        <div>
          <h3 class="text-2xl font-bold">Academic Projects</h3>

          <p class="text-violet-600 font-medium mt-2">College Projects</p>
        </div>

        <span class="text-gray-500 font-bold"> 2025 </span>
      </div>

      <ul class="mt-6 space-y-3 text-gray-600 list-disc pl-5">
        <li>Developed an Attendance Management System.</li>

        <li>
          Created responsive web interfaces using HTML, CSS and JavaScript.
        </li>

        <li>Worked with PHP and MySQL for backend development.</li>
      </ul>
    </div>
  </div>
</section>

<section
  id="skills"
  class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py:16 md:py-20 lg:py-24"
>
  <div class="text-center mb-16">
    <p class="uppercase tracking-[6px] text-violet-600 text-sm font-semibold">
      Skills
    </p>

    <h2 class="text-3xl md:tex-4xl lg:text-5xl font-bold text-gray-900 mt-3">
      Technical Skills
    </h2>

    <p class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base">
      Technologies and tools I use to create modern, responsive, and
      user-friendly web applications.
    </p>
  </div>

  <div class="slider">
    <div class="slide-track">
      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/thumbnails/001/416/705/small/html5-emblem-orange-shield-and-white-text-vector.jpg"
          alt="HTML"
        />
        <h3>HTML</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://cdn-icons-png.flaticon.com/512/919/919826.png"
          alt="CSS"
        />
        <h3>CSS</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/previews/027/127/463/non_2x/javascript-logo-javascript-icon-transparent-free-png.png"
          alt="JavaScript"
        />
        <h3>JavaScript</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/previews/067/565/433/non_2x/tailwind-css-logo-rounded-free-png.png"
          alt="Tailwind"
        />
        <h3>Tailwind CSS</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvC2-syC8tluKeQ3HFmVYdT3JICguDTWb-JIBohqp-Os5NCOlO9EoGBTA&s=10"
          alt="Svelte"
        />
        <h3>SvelteKit</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://banner2.cleanpng.com/20180519/svv/avq1h0vqe.webp"
          alt="MySQL"
        />
        <h3>MySQL</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://cdn.pixabay.com/photo/2022/01/30/13/33/github-6980894_1280.png"
          alt="GitHub"
        />
        <h3>GitHub</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/thumbnails/001/416/705/small/html5-emblem-orange-shield-and-white-text-vector.jpg"
          alt="HTML"
        />
        <h3>HTML</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTj9YYrifS7VtcmWaIucVzhkJ0lI-KNCcyTd635V0w_Cg&s"
          alt="CSS"
        />
        <h3>CSS</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/previews/027/127/463/non_2x/javascript-logo-javascript-icon-transparent-free-png.png"
          alt="JavaScript"
        />
        <h3>JavaScript</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://static.vecteezy.com/system/resources/previews/067/565/433/non_2x/tailwind-css-logo-rounded-free-png.png"
          alt="Tailwind"
        />
        <h3>Tailwind CSS</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvC2-syC8tluKeQ3HFmVYdT3JICguDTWb-JIBohqp-Os5NCOlO9EoGBTA&s=10"
          alt="Svelte"
        />
        <h3>SvelteKit</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://banner2.cleanpng.com/20180519/svv/avq1h0vqe.webp"
          alt="MySQL"
        />
        <h3>MySQL</h3>
      </div>

      <div class="skill-card">
        <img
          src="https://cdn.pixabay.com/photo/2022/01/30/13/33/github-6980894_1280.png"
          alt="GitHub"
        />
        <h3>GitHub</h3>
      </div>
    </div>
  </div>
</section>

<section
  id="contact"
  class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py-16 md:py-20 lg:py-24"
>
  <div class="text-center mb-16">
    <p class="uppercase tracking-[6px] text-violet-600 text-sm font-semibold">
      Contact
    </p>

    <h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-900 mt-3">
      Get In Touch
    </h2>

    <p class="text-gray-500 mt-4 max-w-2xl mx-auto text-sm md:text-base">
      Have a project in mind or want to work together? Feel free to contact me.
      I'm always open to discussing new opportunities.
    </p>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-12 items-start">
    <div class="space-y-8">
      <div class="rounded-3xl border border-gray-300 p-6 md:p-8">
        <h3 class="text-2xl md:text-3xl font-bold mb-6">Contact Information</h3>

        <div class="space-y-6">
          <div>
            <p class="text-gray-400 text-sm">Email</p>
            <h4 class="text-base md:text-lg font-semibold break-all">
              sarswaturvashi01@gmail.com
            </h4>
          </div>

          <div>
            <p class="text-gray-400 text-sm">Phone</p>
            <h4 class="text-lg font-semibold">+91 9457086140</h4>
          </div>

          <div>
            <p class="text-gray-400 text-sm">Location</p>
            <h4 class="text-lg font-semibold">Aligarh Uttar Pradesh, India</h4>
          </div>
        </div>
      </div>
    </div>

    <form
      class="rounded-3xl border border-gray-300 p-6 md:p-8 space-y-5 md:space-y-6"
    >
      <input
        type="text"
        placeholder="Full Name"
        class="w-full border border-gray-300 rounded-xl px-4 md:px-5 py-3 md:py-4 outline-none focus:border-violet-600"
      />

      <input
        type="email"
        placeholder="Email Address"
        class="w-full border border-gray-300 rounded-xl px-4 md:px-5 py-3 md:py-4 outline-none focus:border-violet-600"
      />

      <input
        type="text"
        placeholder="Subject"
        class="w-full border border-gray-300 rounded-xl px-4 md:px-5 py-3 md:py-4 outline-none focus:border-violet-600"
      />

      <textarea
        rows="6"
        placeholder="Write your message..."
        class="w-full border border-gray-300 rounded-xl px-5 py-4 outline-none focus:border-violet-600"
      ></textarea>

      <button
        class="w-full bg-violet-600 text-white py-3 md:py-4 rounded-xl font-semibold text-sm md:text-base hover:bg-violet-700 transition"
      >
        Send Message
      </button>
    </form>
  </div>
</section>

<footer class="border-t border-gray-300 mt-24">
  <div class="max-w-7xl mx-auto px-5 md:px-8 lg:px-12 py-12">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-10">
      <div>
        <h2 class="text-3xl font-bold text-gray-900">
          Urvashi<span class="text-violet-600">.</span>
        </h2>

        <p class="mt-4 text-gray-500">
          Frontend Developer passionate about creating modern, responsive and
          user-friendly web applications using the latest web technologies.
        </p>
      </div>

      <div>
        <h3 class="text-xl font-semibold mb-5">Quick Links</h3>

        <ul class="space-y-3 text-gray-500">
          <li>
            <a href="#services" class="hover:text-violet-600 transition">
              Services
            </a>
          </li>

          <li>
            <a href="#portfolio" class="hover:text-violet-600 transition">
              Portfolio
            </a>
          </li>

          <li>
            <a href="#education" class="hover:text-violet-600 transition">
              Education
            </a>
          </li>

          <li>
            <a href="#experience" class="hover:text-violet-600 transition">
              Experience
            </a>
          </li>

          <li>
            <a href="#contact" class="hover:text-violet-600 transition">
              Contact
            </a>
          </li>
        </ul>
      </div>

      <div>
        <h3 class="text-xl font-semibold mb-5">Contact</h3>

        <div class="space-y-3 text-gray-500">
          <p>📧 sarswaturvashi01@gmail.com</p>
          <p>📞 +91 9457086140</p>
          <p>📍 Aligarh Uttar Pradesh, India</p>
        </div>
      </div>
    </div>

    <div
      class="mt-10 pt-6 border-t border-gray-300 flex flex-col md:flex-row items-center justify-between gap-4"
    >
      <p class="text-blue-400 text-sm text-center md:text-left">
        © 2026 Urvashi Sarswat. All Rights Reserved.
      </p>

      <div class="flex items-center gap-5">
        <a
          href="https://github.com/"
          target="_blank"
          class="text-blue-500 font-bold hover:text-green-500 transition"
        >
          GitHub
        </a>

        <a
          href="https://linkedin.com/"
          target="_blank"
          class="text-blue-500 font-bold hover:text-green-500 transition"
        >
          LinkedIn
        </a>

        <a
          href="mailto:yourmail@gmail.com"
          class="text-blue-500 font-bold hover:text-green-500 transition"
        >
          Email
        </a>
      </div>
    </div>
  </div>
</footer>
