# Portfolio
.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Electrical Engineer Portfolio</title>
    <style>
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --accent-color: #38bdf8; /* Electric Blue */
            --accent-hover: #7dd3fc;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        header {
            text-align: center;
            margin-bottom: 4rem;
        }

        header h1 {
            font-size: 2.5rem;
            color: var(--text-main);
            margin-bottom: 0.5rem;
        }

        header .subtitle {
            font-size: 1.2rem;
            color: var(--accent-color);
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        header .bio {
            max-width: 600px;
            margin: 1.5rem auto 0 auto;
            color: var(--text-muted);
        }

        section {
            margin-bottom: 4rem;
        }

        section h2 {
            font-size: 1.8rem;
            border-bottom: 2px solid var(--card-bg);
            padding-bottom: 0.5rem;
            margin-bottom: 2rem;
            color: var(--text-main);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
        }

        .skills-category {
            background-color: var(--card-bg);
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 4px solid var(--accent-color);
        }

        .skills-category h3 {
            font-size: 1.1rem;
            margin-bottom: 0.75rem;
            color: var(--text-main);
        }

        .skills-category ul {
            list-style: none;
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .skills-category li {
            margin-bottom: 0.4rem;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }

        @media (min-width: 768px) {
            .projects-grid {
                grid-template-columns: 1fr 1fr;
            }
        }

        .project-card {
            background-color: var(--card-bg);
            border-radius: 8px;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            border: 1px solid #334155;
            transition: transform 0.2s, border-color 0.2s;
        }

        .project-card:hover {
            transform: translateY(-4px);
            border-color: var(--accent-color);
        }

        .project-content {
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .project-title {
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: var(--text-main);
        }

        .project-description {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 1.5rem;
            flex-grow: 1;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tag {
            background-color: #0f172a;
            color: var(--accent-color);
            padding: 0.25rem 0.75rem;
            border-radius: 4px;
            font-size: 0.8rem;
            font-weight: 500;
        }

        footer {
            text-align: center;
            margin-top: 6rem;
            padding-top: 2rem;
            border-top: 1px solid var(--card-bg);
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        footer a {
            color: var(--accent-color);
            text-decoration: none;
            margin: 0 0.5rem;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- Header / Introduction -->
        <header>
            <h1>Alex Mercer</h1>
            <div class="subtitle">Electrical Engineer</div>
            <p class="bio">
                Specializing in embedded systems, PCB design, and power electronics. 
                Passionate about designing efficient hardware architecture and bringing complex systems to life.
            </p>
        </header>

        <!-- Technical Skills Section -->
        <section id="skills">
            <h2>Technical Skills</h2>
            <div class="skills-grid">
                <div class="skills-category">
                    <h3>Hardware & PCB Design</h3>
                    <ul>
                        <li>Altium Designer / KiCad</li>
                        <li>Multilayer PCB Layout</li>
                        <li>Signal Integrity</li>
                        <li>High-Power Routing</li>
                    </ul>
                </div>
                <div class="skills-category">
                    <h3>Embedded Systems</h3>
                    <ul>
                        <li>C / C++ Programming</li>
                        <li>ARM Cortex-M (STM32)</li>
                        <li>I2C, SPI, UART, CAN</li>
                        <li>RTOS Architecture</li>
                    </ul>
                </div>
                <div class="skills-category">
                    <h3>Testing & Tools</h3>
                    <ul>
                        <li>Oscilloscopes / Logic Analyzers</li>
                        <li>SPICE Simulation (LTspice)</li>
                        <li>MATLAB / Simulink</li>
                        <li>LabVIEW</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects">
            <h2>Featured Projects</h2>
            <div class="projects-grid">
                
                <!-- Project 1 -->
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Autonomous Drone Power Distribution Management</h3>
                        <p class="project-description">
                            Designed and tested a 4-layer power management board optimized for industrial quadcopters. 
                            Features active cell balancing, overcurrent protection circuits, and high-efficiency buck-boost regulation to extend battery lifespans.
                        </p>
                        <div class="project-tags">
                            <span class="tag">KiCad</span>
                            <span class="tag">Power Electronics</span>
                            <span class="tag">LTspice</span>
                        </div>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">STM32 IoT Environmental Sensor Hub</h3>
                        <p class="project-description">
                            Developed firmware and hardware for a low-power telemetry station. Utilized an ARM Cortex-M micro-controller to poll sensor grids over I2C and transmit data via a cellular module.
                        </p>
                        <div class="project-tags">
                            <span class="tag">Embedded C</span>
                            <span class="tag">STM32</span>
                            <span class="tag">Altium</span>
                        </div>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Brushless DC (BLDC) Motor Controller</h3>
                        <p class="project-description">
                            Built a custom 3-phase inverter board with a field-oriented control (FOC) algorithm implemented on an MCU. Achieved smooth variable speed loops with regenerative braking capability.
                        </p>
                        <div class="project-tags">
                            <span class="tag">FOC</span>
                            <span class="tag">MOSFETs</span>
                            <span class="tag">Firmware</span>
                        </div>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Industrial Automation PLC Interfacing</h3>
                        <p class="project-description">
                            Designed noise-isolated digital and analog I/O expansion modules for harsh electrical environments, implementing optocouplers to guarantee signal protection.
                        </p>
                        <div class="project-tags">
                            <span class="tag">Isolation</span>
                            <span class="tag">Analog Design</span>
                            <span class="tag">EMC Testing</span>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <!-- Footer / Contact Info -->
        <footer>
            <p>Connect with me:</p>
