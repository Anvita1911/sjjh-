<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Sea Turtle Conservation</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background: url('https://images.unsplash.com/photo-1530213786676-35c8c0b4e5d3') no-repeat center center fixed;
      background-size: cover;
      color: #ffffff;
    }

    header {
      background-color: rgba(0, 51, 102, 0.8);
      padding: 50px 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 3em;
    }

    nav {
      background-color: rgba(0, 102, 153, 0.8);
      text-align: center;
      padding: 10px 0;
    }

    nav button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      background-color: #00b4d8;
      border: none;
      border-radius: 5px;
      color: white;
      cursor: pointer;
    }

    nav button:hover {
      background-color: #0077b6;
    }

    main {
      padding: 30px;
      max-width: 900px;
      margin: auto;
      background-color: rgba(0, 0, 51, 0.7);
      border-radius: 10px;
    }

    section {
      display: none;
      animation: fadeIn 0.5s ease-in-out;
    }

    section.active {
      display: block;
    }

    h2 {
      border-bottom: 2px solid #00b4d8;
      padding-bottom: 10px;
    }

    img {
      max-width: 100%;
      border-radius: 10px;
      margin: 20px 0;
    }

    footer {
      text-align: center;
      background-color: rgba(0, 51, 102, 0.8);
      padding: 20px;
      color: #ffffff;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .quiz {
      margin-top: 20px;
    }

    .quiz input[type="radio"] {
      margin-right: 10px;
    }

    .quiz-result {
      margin-top: 10px;
      font-weight: bold;
      color: #00ffcc;
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://cdn.pixabay.com/audio/2022/08/04/audio_9755bdf0a6.mp3" type="audio/mpeg">
  </audio>

  <header>
    <h1>Save the Sea Turtles</h1>
    <p>Learn. Protect. Act.</p>
  </header>

  <nav>
    <button onclick="showSection('home')">Home</button>
    <button onclick="showSection('species')">Species</button>
    <button onclick="showSection('threats')">Threats</button>
    <button onclick="showSection('conservation')">Conservation</button>
    <button onclick="showSection('help')">How You Can Help</button>
    <button onclick="showSection('quiz')">Turtle Quiz!</button>
  </nav>

  <main>
    <section id="home" class="active">
      <h2>Welcome</h2>
      <p>Sea turtles have graced our oceans for over 100 million years. But now, they face grave dangers from human activities. Explore this site to learn more about the different species, threats they face, and how you can make a difference.</p>
      <img src="https://upload.wikimedia.org/wikipedia/commons/4/41/Sea_turtle_grazing_seagrass.jpg" alt="Sea Turtle Grazing" />
    </section>

    <section id="species">
      <h2>Sea Turtle Species</h2>
      <p>There are 7 known species of sea turtles:</p>
      <ul>
        <li><strong>Leatherback</strong> – the largest and can dive up to 4,000 feet deep!</li>
        <li><strong>Green</strong> – known for their greenish fat and herbivorous diet</li>
        <li><strong>Loggerhead</strong> – powerful jaws for crushing prey like crabs</li>
        <li><strong>Hawksbill</strong> – has a beautiful shell and feeds on sponges</li>
        <li><strong>Olive Ridley</strong> – smallest sea turtle, known for mass nesting events</li>
        <li><strong>Kemp’s Ridley</strong> – critically endangered, nests during the day</li>
        <li><strong>Flatback</strong> – found only in Australia’s coastal waters</li>
      </ul>
      <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/Sea_turtle_swimming_over_coral_reef.jpg" alt="Sea Turtle swimming" />
    </section>

    <section id="threats">
      <h2>Threats They Face</h2>
      <p>Sea turtles face multiple threats, mostly caused by humans:</p>
      <ul>
        <li><strong>Plastic Pollution:</strong> Turtles often mistake plastic for jellyfish.</li>
        <li><strong>Fishing Bycatch:</strong> Turtles get accidentally caught in fishing gear.</li>
        <li><strong>Climate Change:</strong> Rising sand temperatures affect hatchling gender.</li>
        <li><strong>Loss of Nesting Habitat:</strong> Due to beachfront development.</li>
        <li><strong>Poaching:</strong> Turtle shells and eggs are illegally sold.</li>
      </ul>
      <img src="https://upload.wikimedia.org/wikipedia/commons/e/e1/Sea_turtle_in_plastic_pollution.jpg" alt="Turtle and Plastic Pollution" />
    </section>

    <section id="conservation">
      <h2>Conservation Efforts</h2>
      <p>Organizations and communities worldwide are taking action:</p>
      <ul>
        <li>Protecting nesting beaches</li>
        <li>Educating locals and tourists</li>
        <li>Tracking turtles with satellite tags</li>
        <li>Passing laws against illegal trade</li>
        <li>Cleaning oceans and reducing plastic</li>
      </ul>
      <img src="https://upload.wikimedia.org/wikipedia/commons/3/3e/Olive_Ridley_Sea_Turtle_Tagging.jpg" alt="Sea turtle conservation tagging" />
    </section>

    <section id="help">
      <h2>How You Can Help</h2>
      <ul>
        <li>Reduce plastic use – especially straws and bags</li>
        <li>Participate in beach cleanups</li>
        <li>Donate to ocean conservation organizations</li>
        <li>Keep beaches dark during nesting season</li>
        <li>Spread awareness about sea turtle protection</li>
      </ul>
      <img src="https://upload.wikimedia.org/wikipedia/commons/4/47/Turtle_conservation_Malaysia.jpg" alt="Volunteers helping turtles" />
    </section>

    <section id="quiz">
      <h2>🐢 Turtle Trivia!</h2>
      <div class="quiz">
        <p>1. Which is the largest sea turtle species?</p>
        <label><input type="radio" name="q1" value="a">Green Turtle</label><br>
        <label><input type="radio" name="q1" value="b">Leatherback</label><br>
        <label><input type="radio" name="q1" value="c">Hawksbill</label>

        <p>2. What do sea turtles often mistake plastic bags for?</p>
        <label><input type="radio" name="q2" value="a">Fish</label><br>
        <label><input type="radio" name="q2" value="b">Algae</label><br>
        <label><input type="radio" name="q2" value="c">Jellyfish</label>

        <p><button onclick="checkQuiz()">Check Answers</button></p>
        <div class="quiz-result" id="quiz-result"></div>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2025 Sea Turtle Conservation Project 🐢
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll("section").forEach(section => {
        section.classList.remove("active");
      });
      document.getElementById(id).classList.add("active");
      window.scrollTo({ top: 0, behavior: "smooth" });
    }

    function checkQuiz() {
      let score = 0;
      if (document.querySelector('input[name="q1"]:checked')?.value === "b") score++;
      if (document.querySelector('input[name="q2"]:checked')?.value === "c") score++;
      document.getElementById("quiz-result").innerText = `You got ${score}/2 correct! 🐢`;
    }
  </script>
</body>
</html>
