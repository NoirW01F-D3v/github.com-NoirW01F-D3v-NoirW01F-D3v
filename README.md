<?xml version="1.0" encoding="UTF-8"?>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 5200" width="900" height="5200">
  <defs>
    <linearGradient id="headerGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#FF6B6B"/>        <stop offset="50%" stop-color="#4ECDC4"/>
      <stop offset="100%" stop-color="#45B7D1"/>    </linearGradient>
    <linearGradient id="cardGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#FFFFFF"/>        <stop offset="100%" stop-color="#F0F9FF"/>
    </linearGradient>                               <linearGradient id="tipGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#FFE66D"/>        <stop offset="100%" stop-color="#FF9F43"/>
    </linearGradient>
    <linearGradient id="codeGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#1E1E2E"/>
      <stop offset="100%" stop-color="#2A2A3C"/>
    </linearGradient>
    <filter id="shadow" x="-20%" y="-20%" width="140%" height="140%">
      <feDropShadow dx="3" dy="4" stdDeviation="4" flood-color="#00000033"/>
    </filter>
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="5200" fill="#F8FAFC"/>

  <!-- Decorative circles -->
  <circle cx="50" cy="80" r="40" fill="#FF6B6B" opacity="0.15"/>
  <circle cx="850" cy="150" r="60" fill="#4ECDC4" opacity="0.15"/>
  <circle cx="100" cy="800" r="30" fill="#45B7D1" opacity="0.1"/>
  <circle cx="820" cy="1600" r="50" fill="#FFE66D" opacity="0.15"/>
  <circle cx="70" cy="2800" r="45" fill="#FF9F43" opacity="0.12"/>
  <circle cx="830" cy="3800" r="55" fill="#4ECDC4" opacity="0.12"/>
  <circle cx="60" cy="4800" r="35" fill="#FF6B6B" opacity="0.1"/>

  <!-- ========== HEADER ========== -->
  <rect x="0" y="0" width="900" height="220" fill="url(#headerGrad)"/>
  <text x="450" y="70" font-family="Arial, Helvetica, sans-serif" font-size="36" font-weight="bold" fill="white" text-anchor="middle">🎉 Your First Gradle App in Termux!</mathrm>
  <text x="450" y="115" font-family="Arial, Helvetica, sans-serif" font-size="20" fill="white" text-anchor="middle" opacity="0.95">A joyful GitHub-style tutorial for absolute beginners</text>
  <text x="450" y="155" font-family="Arial, Helvetica, sans-serif" font-size="16" fill="white" text-anchor="middle" opacity="0.9">Learn by doing • Fun details • Real tips • Pure joy</text>
  <text x="450" y="195" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="white" text-anchor="middle" opacity="0.85">Made with ❤️ for Termux explorers</text>

  <!-- ========== INTRO CARD ========== -->
  <rect x="40" y="250" width="820" height="280" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <text x="70" y="295" font-family="Arial, Helvetica, sans-serif" font-size="24" font-weight="bold" fill="#1E293B">🚀 Welcome, future app maker!</text>
  <text x="70" y="335" font-family="Arial, Helvetica, sans-serif" font-size="16" fill="#334155">
    <tspan x="70" dy="0">You are about to create your very first real application using</tspan>
    <tspan x="70" dy="26">Gradle — the powerful build tool that professionals love.</tspan>
    <tspan x="70" dy="26">We will do it entirely inside Termux on your Android phone.</tspan>
    <tspan x="70" dy="26">No computer needed. No Android Studio. Just pure terminal magic.</tspan>
  </text>
  <text x="70" y="470" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#0F766E" font-weight="bold">
    What you will build today: A simple Java “Hello” app that runs with one command.
  </text>
  <text x="70" y="500" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#64748B">
    Ready? Let’s turn your phone into a tiny developer machine. ✨
  </text>

  <!-- ========== TIP BUBBLE 1 ========== -->
  <rect x="40" y="560" width="820" height="110" rx="16" fill="url(#tipGrad)" filter="url(#shadow)"/>
  <text x="70" y="600" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="#7C2D12">💡 Pro Tip #1 — Why Gradle?</text>
  <text x="70" y="635" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#9A3412">
    <tspan x="70" dy="0">Gradle is not just “another tool”. It automatically downloads libraries, compiles code,</tspan>
    <tspan x="70" dy="22">runs tests, and packages your app. Once you learn it here, you can use the same skills</tspan>
    <tspan x="70" dy="22">for Android apps, Kotlin, Spring, and almost every modern Java project.</tspan>
  </text>

  <!-- ========== STEP 1 ========== -->
  <rect x="40" y="700" width="820" height="420" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <circle cx="80" cy="745" r="22" fill="#4ECDC4"/>
  <text x="80" y="752" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="white" text-anchor="middle">1</text>
  <text x="120" y="755" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">Install the essentials</text>

  <text x="70" y="800" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    Open Termux and paste these two lines. They update packages and install Java + Gradle.
  </text>

  <!-- Code box -->
  <rect x="60" y="820" width="780" height="130" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="850" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">pkg update -y &amp;&amp; pkg upgrade -y</text>
  <text x="80" y="880" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">pkg install openjdk-21 gradle git wget unzip -y</text>
  <text x="80" y="920" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA"># This gives you Java 21 (modern) and the latest Gradle</text>

  <text x="70" y="980" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#0F766E" font-weight="bold">Verify it worked:</text>
  <rect x="60" y="995" width="780" height="90" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="1025" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">java -version</text>
  <text x="80" y="1055" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">gradle -v</text>

  <!-- ========== TIP 2 ========== -->
  <rect x="40" y="1150" width="820" height="100" rx="16" fill="#E0F2FE" filter="url(#shadow)"/>
  <text x="70" y="1185" font-family="Arial, Helvetica, sans-serif" font-size="16" font-weight="bold" fill="#0369A1">🧠 Detail worth knowing</text>
  <text x="70" y="1215" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#0C4A6E">
    openjdk-21 is the Long-Term Support version. Gradle 8+/9+ loves it. If something fails later, always check java -version first!
  </text>

  <!-- ========== STEP 2 ========== -->
  <rect x="40" y="1280" width="820" height="380" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <circle cx="80" cy="1325" r="22" fill="#FF6B6B"/>
  <text x="80" y="1332" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="white" text-anchor="middle">2</text>
  <text x="120" y="1335" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">Create your project (the fun part!)</text>

  <text x="70" y="1380" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    This single command creates a full professional project structure for you.
  </text>

  <rect x="60" y="1400" width="780" height="160" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="1430" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">mkdir ~/MyFirstApp &amp;&amp; cd ~/MyFirstApp</text>
  <text x="80" y="1460" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">gradle init --type java-application --dsl groovy \</text>
  <text x="80" y="1485" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">  --test-framework junit-jupiter \</text>
  <text x="80" y="1510" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">  --project-name MyFirstApp --package com.example</text>
  <text x="80" y="1540" font-family="Consolas, Monaco, monospace" font-size="12" fill="#89B4FA"># Press Enter on the questions — defaults are perfect for beginners</text>

  <text x="70" y="1600" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#64748B">
    Gradle will generate folders, build files, a sample main class, and even tests. Magic!
  </text>

  <!-- ========== STEP 3 ========== -->
  <rect x="40" y="1690" width="820" height="480" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <circle cx="80" cy="1735" r="22" fill="#FFE66D"/>
  <text x="80" y="1742" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="#7C2D12" text-anchor="middle">3</text>
  <text x="120" y="1745" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">Write your first real code</text>

  <text x="70" y="1790" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    Open the main file with nano (simple editor that comes with Termux):
  </text>

  <rect x="60" y="1810" width="780" height="50" rx="10" fill="url(#codeGrad)"/>
  <text x="80" y="1842" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">nano app/src/main/java/com/example/App.java</text>

  <text x="70" y="1890" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#334155">Delete everything inside and paste this joyful version:</text>

  <rect x="60" y="1910" width="780" height="200" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="1940" font-family="Consolas, Monaco, monospace" font-size="13" fill="#CBA6F7">package com.example;</text>
  <text x="80" y="1970" font-family="Consolas, Monaco, monospace" font-size="13" fill="#F9E2AF"></text>
  <text x="80" y="1995" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA">public class App {</text>
  <text x="100" y="2025" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA">public static void main(String[] args) {</text>
  <text x="120" y="2055" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">System.out.println("Hello from Gradle + Termux!");</text>
  <text x="120" y="2080" font-family="Consolas, Monaco, monospace" font-size="13" fill="#A6E3A1">System.out.println("This is my first app 🎉");</text>
  <text x="100" y="2105" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA">}</text>
  <text x="80" y="2130" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA">}</text>

  <!-- ========== TIP 3 ========== -->
  <rect x="40" y="2200" width="820" height="130" rx="16" fill="url(#tipGrad)" filter="url(#shadow)"/>
  <text x="70" y="2240" font-family="Arial, Helvetica, sans-serif" font-size="17" font-weight="bold" fill="#7C2D12">💾 How to save in nano</text>
  <text x="70" y="2275" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#9A3412">
    <tspan x="70" dy="0">1. Press Ctrl + O  (write Out)</tspan>
    <tspan x="70" dy="22">2. Press Enter to confirm the filename</tspan>
    <tspan x="70" dy="22">3. Press Ctrl + X to exit. You are now a nano ninja!</tspan>
  </text>

  <!-- ========== STEP 4 ========== -->
  <rect x="40" y="2360" width="820" height="320" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <circle cx="80" cy="2405" r="22" fill="#4ECDC4"/>
  <text x="80" y="2412" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="white" text-anchor="middle">4</text>
  <text x="120" y="2415" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">Run your app — the magic moment</text>

  <text x="70" y="2460" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    From inside the MyFirstApp folder, simply type:
  </text>

  <rect x="60" y="2480" width="780" height="80" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="2515" font-family="Consolas, Monaco, monospace" font-size="16" fill="#A6E3A1">./gradlew run</text>
  <text x="80" y="2545" font-family="Consolas, Monaco, monospace" font-size="13" fill="#89B4FA"># or just:  gradle run</text>

  <text x="70" y="2600" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#0F766E" font-weight="bold">
    You should see:
  </text>
  <text x="70" y="2630" font-family="Consolas, Monaco, monospace" font-size="15" fill="#1E293B">
    Hello from Gradle + Termux!
  </text>
  <text x="70" y="2655" font-family="Consolas, Monaco, monospace" font-size="15" fill="#1E293B">
    This is my first app 🎉
  </text>

  <!-- ========== CELEBRATION ========== -->
  <rect x="40" y="2710" width="820" height="160" rx="20" fill="#DCFCE7" filter="url(#shadow)"/>
  <text x="450" y="2770" font-family="Arial, Helvetica, sans-serif" font-size="28" font-weight="bold" fill="#166534" text-anchor="middle">🎊 CONGRATULATIONS! 🎊</text>
  <text x="450" y="2815" font-family="Arial, Helvetica, sans-serif" font-size="16" fill="#15803D" text-anchor="middle">
    You just built, compiled, and ran a real Java application with Gradle
  </text>
  <text x="450" y="2845" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#166534" text-anchor="middle">
    on an Android phone. That is seriously cool.
  </text>

  <!-- ========== STEP 5 - BONUS ========== -->
  <rect x="40" y="2900" width="820" height="300" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <circle cx="80" cy="2945" r="22" fill="#A78BFA"/>
  <text x="80" y="2952" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="white" text-anchor="middle">5</text>
  <text x="120" y="2955" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">Bonus: Make a runnable JAR</text>

  <text x="70" y="3000" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    Package your app so anyone can run it with just Java:
  </text>

  <rect x="60" y="3020" width="780" height="100" rx="12" fill="url(#codeGrad)"/>
  <text x="80" y="3055" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">./gradlew jar</text>
  <text x="80" y="3085" font-family="Consolas, Monaco, monospace" font-size="14" fill="#A6E3A1">java -jar app/build/libs/app-1.0-SNAPSHOT.jar</text>

  <text x="70" y="3160" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#64748B">
    The JAR file lives in app/build/libs/ — you can even share it!
  </text>

  <!-- ========== TIPS SECTION ========== -->
  <rect x="40" y="3230" width="820" height="520" rx="20" fill="#FEF3C7" filter="url(#shadow)"/>
  <text x="70" y="3280" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#92400E">🌟 Joyful Tips &amp; Little Details</text>

  <text x="70" y="3330" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• Why ./gradlew instead of gradle?</text>
  <text x="70" y="3355" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    The wrapper (gradlew) guarantees everyone uses the exact same Gradle version. Super professional habit!
  </text>

  <text x="70" y="3400" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• Folder structure is your friend</text>
  <text x="70" y="3425" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    src/main/java → your real code  src/test/java → tests  build.gradle → the recipe
  </text>

  <text x="70" y="3470" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• First build is slow — that’s normal</text>
  <text x="70" y="3495" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    Gradle downloads the world the first time. Next runs are lightning fast thanks to its clever cache.
  </text>

  <text x="70" y="3540" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• Want a better editor?</text>
  <text x="70" y="3565" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    pkg install micro  or  pkg install neovim  — both feel great on a phone keyboard.
  </text>

  <text x="70" y="3610" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• Keep projects in ~/ (home)</text>
  <text x="70" y="3635" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    Termux home is the fastest and safest place. Avoid /sdcard for build folders if you can.
  </text>

  <text x="70" y="3680" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#78350F" font-weight="bold">• Explore the files!</text>
  <text x="70" y="3705" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#92400E">
    Open build.gradle and settings.gradle with nano. Reading them is how you really learn Gradle.
  </text>

  <!-- ========== NEXT LEVEL ========== -->
  <rect x="40" y="3780" width="820" height="280" rx="20" fill="url(#cardGrad)" filter="url(#shadow)"/>
  <text x="70" y="3830" font-family="Arial, Helvetica, sans-serif" font-size="22" font-weight="bold" fill="#1E293B">🚀 Ready for the next adventure?</text>
  <text x="70" y="3875" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    Once this feels easy, you can level up to building real Android APKs entirely in Termux.
  </text>
  <text x="70" y="3910" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#334155">
    That needs the Android SDK + a tiny aapt2 fix, but the same Gradle skills apply.
  </text>
  <text x="70" y="3955" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#0F766E" font-weight="bold">
    Search for “termux-build-apps” on GitHub for ready-made setup scripts when you’re ready.
  </text>
  <text x="70" y="3995" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#64748B">
    Or come back and ask for the full Android Hello World SVG lesson!
  </text>

  <!-- ========== FOOTER ========== -->
  <rect x="0" y="4100" width="900" height="200" fill="#1E293B"/>
  <text x="450" y="4160" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="bold" fill="white" text-anchor="middle">You did it. You are now a Gradle beginner with real skills.</text>
  <text x="450" y="4200" font-family="Arial, Helvetica, sans-serif" font-size="15" fill="#94A3B8" text-anchor="middle">Share this SVG tutorial on GitHub • Star it • Remix it • Teach a friend</text>
  <text x="450" y="4240" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#64748B" text-anchor="middle">Made with joy for the Termux community  •  2026</text>
  <text x="450" y="4275" font-family="Arial, Helvetica, sans-serif" font-size="13" fill="#475569" text-anchor="middle">Open this .svg in any browser or GitHub — it stays crisp forever</text>

  <!-- Decorative stars -->
  <text x="80" y="4350" font-size="24" fill="#FFE66D">★</text>
  <text x="200" y="4380" font-size="18" fill="#4ECDC4">★</text>
  <text x="700" y="4360" font-size="22" fill="#FF6B6B">★</text>
  <text x="820" y="4390" font-size="16" fill="#A78BFA">★</text>

  <!-- Final message -->
  <text x="450" y="4480" font-family="Arial, Helvetica, sans-serif" font-size="20" font-weight="bold" fill="#1E293B" text-anchor="middle">Keep building. Keep smiling. The terminal is your playground.</text>
  <text x="450" y="4530" font-family="Arial, Helvetica, sans-serif" font-size="28" fill="#4ECDC4" text-anchor="middle">✨ Happy coding! ✨</text>

  <!-- Tiny robot illustration (simple shapes) -->
  <g transform="translate(400, 4620)">
    <rect x="-30" y="0" width="60" height="50" rx="8" fill="#4ECDC4"/>
    <circle cx="-15" cy="20" r="6" fill="#1E293B"/>
    <circle cx="15" cy="20" r="6" fill="#1E293B"/>
    <rect x="-10" y="32" width="20" height="6" rx="3" fill="#1E293B"/>
    <rect x="-40" y="15" width="10" height="20" rx="3" fill="#45B7D1"/>
    <rect x="30" y="15" width="10" height="20" rx="3" fill="#45B7D1"/>
    <rect x="-20" y="50" width="12" height="20" rx="3" fill="#FF6B6B"/>
    <rect x="8" y="50" width="12" height="20" rx="3" fill="#FF6B6B"/>
  </g>
  <text x="450" y="4740" font-family="Arial, Helvetica, sans-serif" font-size="13" fill="#64748B" text-anchor="middle">Your new coding buddy says: “You got this!”</text>

  <!-- GitHub style note -->
  <text x="450" y="4850" font-family="Arial, Helvetica, sans-serif" font-size="14" fill="#94A3B8" text-anchor="middle">This entire lesson is one pure SVG file — perfect for GitHub READMEs or gists.</text>
  <text x="450" y="4890" font-family="Arial, Helvetica, sans-serif" font-size="13" fill="#64748B" text-anchor="middle">Just upload First-Gradle-App-Termux-Tutorial.svg and enjoy the colorful journey.</text>

  <!-- End decorative line -->
  <line x1="100" y1="5000" x2="800" y2="5000" stroke="#CBD5E1" stroke-width="2"/>
  <text x="450" y="5050" font-family="Arial, Helvetica, sans-serif" font-size="12" fill="#94A3B8" text-anchor="middle">End of tutorial • Go make something wonderful</text>
</svg>