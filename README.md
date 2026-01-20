<!DOCTYPE html>
<html class="dark" lang="en">

<head>
    <meta charset="utf-8" />
    <meta content="width=device-width, initial-scale=1.0" name="viewport" />
    <title>Billy Cristian Fauji | Systems Architect Portfolio</title>
    <script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;900&amp;display=swap"
        rel="stylesheet" />
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&amp;display=swap"
        rel="stylesheet" />
    <link
        href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap"
        rel="stylesheet" />
    <script id="tailwind-config">
        tailwind.config = {
            darkMode: "class",
            theme: {
                extend: {
                    colors: {
                        "primary": "#00c7c7",
                        "accent-blue": "#0066ff",
                        "background-light": "#f0f0f0",
                        "background-dark": "#0d0d0d",
                        "surface-dark": "#1a1a1a",
                        "border-dark": "#262626",
                        "border-muted": "#666666",
                        "system-green": "#00ff41",
                    },
                    fontFamily: {
                        "display": ["Inter", "sans-serif"],
                        "mono": ["JetBrains Mono", "SF Mono", "monospace"]
                    },
                    borderRadius: {
                        "DEFAULT": "0.125rem",
                        "lg": "0.25rem",
                        "xl": "0.5rem",
                        "full": "0.75rem"
                    },
                },
            },
        }
    </script>
    <style type="text/tailwindcss">
        .technical-grid {
            background-image: radial-gradient(circle, #262626 1px, transparent 1px);
            background-size: 32px 32px;
        }
        .line-pattern {
            background: repeating-linear-gradient(
                90deg,
                #262626,
                #262626 1px,
                transparent 1px,
                transparent 32px
            );
        }
        .illustration-mask {
            mask-image: linear-gradient(to right, transparent, black 20%, black 80%, transparent),
                        linear-gradient(to bottom, transparent, black 15%, black 85%, transparent);
            mask-composite: intersect;
            -webkit-mask-image: linear-gradient(to right, transparent, black 20%, black 80%, transparent),
                               linear-gradient(to bottom, transparent, black 15%, black 85%, transparent);
            -webkit-mask-composite: source-in;
        }
        .ticker-scroll {
            display: flex;
            width: fit-content;
            animation: ticker 30s linear infinite;
        }
        @keyframes ticker {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }
        .pulse-soft {
            animation: pulse-ring 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
        }
        @keyframes pulse-ring {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: .5; transform: scale(1.1); }
        }
    </style>
</head>

<body
    class="bg-background-light dark:bg-background-dark font-display text-white selection:bg-primary selection:text-background-dark pb-12 md:pb-16">
    <header
        class="fixed top-0 w-full z-50 bg-background-light/90 dark:bg-background-dark/90 backdrop-blur-md border-b border-border-muted/30">
        <div class="max-w-[1200px] mx-auto px-6 h-16 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <span class="material-symbols-outlined text-primary text-2xl">account_tree</span>
                <span class="font-black tracking-tighter text-lg dark:text-white text-black">BCF / SYSTEMS</span>
            </div>
            <nav class="hidden md:flex items-center gap-12">
                <a class="text-sm font-medium dark:text-gray-400 dark:hover:text-primary text-gray-600 transition-colors uppercase tracking-widest"
                    href="#systems">[Systems]</a>
                <a class="text-sm font-medium dark:text-gray-400 dark:hover:text-primary text-gray-600 transition-colors uppercase tracking-widest"
                    href="#thinking">[Thinking]</a>
                <a class="text-sm font-medium dark:text-gray-400 dark:hover:text-primary text-gray-600 transition-colors uppercase tracking-widest"
                    href="#contact">[Contact]</a>
                <button
                    class="bg-primary text-background-dark px-5 py-2 text-xs font-bold uppercase tracking-widest hover:brightness-110 transition-all rounded">
                    Let's Talk
                </button>
            </nav>
        </div>
    </header>
    <main class="pt-16">
        <section
            class="relative min-h-[95vh] flex flex-col justify-center px-6 overflow-hidden technical-grid border-b border-border-dark">
            <div
                class="absolute right-0 top-1/2 -translate-y-1/2 w-1/2 h-full opacity-40 lg:opacity-60 mix-blend-luminosity illustration-mask pointer-events-none select-none">
                <!-- <img alt="Stylized Illustration" class="w-full h-full object-cover grayscale contrast-125 brightness-75" src="https://lh3.googleusercontent.com/aida-public/AB6AXuBnmg44oxCOnMYhqquTaEayqrrs7moF-7EGRFmY4ntl41CDXJAdM-tQUm-FRuka0bY9NgfrVpt4Na48iWwgoj2gLkBpbD39fTKQ41kV7DH2rehZICfcL1QgP2FCseRjhb2sNxkthSBiVaqMN9HE_9Zo_P36oXRf0O1GiGzWY_iz6sZS_Q4lkJRwpPc9zZkRBPCIzptIC3VdZlOolHtLnfkyqmC1e8oLdpqUBkMDpFFtaD0tG_oS0HXApAMEbMonqk_RhjUxXraEoAE"/> -->
            </div>
            <div class="max-w-[1200px] mx-auto w-full py-20 relative z-10">
                <div
                    class="absolute top-0 right-0 p-4 border border-border-dark text-[10px] text-border-muted font-mono hidden lg:block uppercase tracking-widest bg-background-dark/50 backdrop-blur-sm">
                    Status: System_Optimal<br />
                    Location: 127.0.0.1<br />
                    Load: 0.08 / 0.12 / 0.05
                </div>
                <div class="max-w-4xl space-y-8">
                    <div
                        class="inline-flex items-center gap-2 px-3 py-1 border border-primary/30 bg-primary/5 text-primary text-[10px] font-bold uppercase tracking-[0.2em]">
                        <span class="relative flex h-2 w-2">
                            <span
                                class="animate-ping absolute inline-flex h-full w-full rounded-full bg-primary opacity-75"></span>
                            <span class="relative inline-flex rounded-full h-2 w-2 bg-primary"></span>
                        </span>
                        Specialized Generalist IT Professional
                    </div>
                    <h1
                        class="text-6xl md:text-8xl font-black leading-[0.9] tracking-tighter dark:text-white text-black drop-shadow-2xl">
                        BILLY CRISTIAN <span class="text-primary">FAUJI</span>
                    </h1>
                    <p
                        class="text-xl md:text-2xl dark:text-gray-400 text-gray-600 max-w-2xl leading-relaxed font-light drop-shadow-lg">
                        I build systems that remove friction, <span
                            class="dark:text-white text-black font-semibold italic">not just code that runs.</span>
                    </p>
                    <div class="flex flex-wrap gap-4 pt-4">
                        <a class="bg-primary text-background-dark px-8 py-4 text-sm font-bold uppercase tracking-widest hover:brightness-110 transition-all flex items-center gap-3 shadow-xl shadow-primary/10"
                            href="#systems">
                            View Systems <span class="material-symbols-outlined text-sm">arrow_forward</span>
                        </a>
                        <a class="border border-border-muted px-8 py-4 text-sm font-bold uppercase tracking-widest hover:bg-white/5 transition-all text-gray-400 backdrop-blur-sm"
                            href="#thinking">
                            The Manifesto
                        </a>
                    </div>
                </div>
            </div>
            <div
                class="absolute bottom-0 left-0 w-full h-[1px] bg-gradient-to-r from-transparent via-border-muted/50 to-transparent">
            </div>
        </section>
        <section class="py-32 px-6 dark:bg-background-dark bg-white" id="thinking">
            <div class="max-w-[1200px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
                <div class="lg:col-span-4">
                    <h2 class="text-xs font-bold text-primary uppercase tracking-[0.3em] mb-6 flex items-center gap-4">
                        <span class="w-8 h-[1px] bg-primary"></span> [Thinking]
                    </h2>
                    <h3 class="text-3xl font-bold dark:text-white text-black leading-tight">Technical Mindset Manifesto
                    </h3>
                </div>
                <div class="lg:col-span-8 space-y-12">
                    <p
                        class="text-3xl md:text-4xl font-semibold dark:text-gray-300 text-gray-800 leading-snug tracking-tight">
                        Efficiency over activity. Stability as a baseline. I approach every project with a <span
                            class="dark:text-white text-black underline decoration-primary decoration-4 underline-offset-8">systems-first
                            methodology</span>, ensuring that every line of code serves a structural purpose.
                    </p>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-8 pt-12 border-t border-border-dark">
                        <div class="space-y-4">
                            <h4 class="font-bold dark:text-white text-black uppercase tracking-widest text-sm italic">
                                01. Reduced Complexity</h4>
                            <p class="text-gray-500 leading-relaxed text-sm">Abstraction is a tool, not a goal. If a
                                system can't be explained simply, it hasn't been designed correctly yet.</p>
                        </div>
                        <div class="space-y-4">
                            <h4 class="font-bold dark:text-white text-black uppercase tracking-widest text-sm italic">
                                02. Frictionless Output</h4>
                            <p class="text-gray-500 leading-relaxed text-sm">Technology should disappear into the
                                workflow. The best systems are those the user forgets are even there.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="py-32 px-6 dark:bg-surface-dark bg-background-light border-y border-border-dark" id="systems">
            <div class="max-w-[1200px] mx-auto">
                <div class="flex justify-between items-end mb-16">
                    <div>
                        <h2
                            class="text-xs font-bold text-primary uppercase tracking-[0.3em] mb-6 flex items-center gap-4">
                            <span class="w-8 h-[1px] bg-primary"></span> [Systems]
                        </h2>
                        <h3 class="text-4xl font-bold dark:text-white text-black">Core Capabilities</h3>
                    </div>
                    <div class="hidden md:block text-right">
                        <span class="text-[10px] font-mono dark:text-border-muted text-gray-400">MODULE_COUNT:
                            04<br />INTEGRATION: FULL</span>
                    </div>
                </div>
                <div
                    class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-px bg-border-dark border border-border-dark">
                    <div class="dark:bg-background-dark bg-white p-10 group hover:dark:bg-surface-dark transition-all">
                        <span class="material-symbols-outlined text-4xl text-primary mb-8 block">layers</span>
                        <h4 class="text-xl font-bold mb-4 dark:text-white text-black uppercase tracking-tighter">
                            Infrastructure</h4>
                        <p class="text-sm dark:text-gray-400 text-gray-600 mb-6 leading-relaxed">Designing scalable
                            foundations that serve as the bedrock for enterprise-level deployment and growth.</p>
                        <div class="flex flex-wrap gap-2">
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">Terraform</span>
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">AWS/GCP</span>
                        </div>
                    </div>
                    <div class="dark:bg-background-dark bg-white p-10 group hover:dark:bg-surface-dark transition-all">
                        <span
                            class="material-symbols-outlined text-4xl text-primary mb-8 block">precision_manufacturing</span>
                        <h4 class="text-xl font-bold mb-4 dark:text-white text-black uppercase tracking-tighter">
                            Automation</h4>
                        <p class="text-sm dark:text-gray-400 text-gray-600 mb-6 leading-relaxed">Removing human error
                            through rigorous CI/CD pipelines and programmatic resource management.</p>
                        <div class="flex flex-wrap gap-2">
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">Ansible</span>
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">GitHub
                                Actions</span>
                        </div>
                    </div>
                    <div class="dark:bg-background-dark bg-white p-10 group hover:dark:bg-surface-dark transition-all">
                        <span class="material-symbols-outlined text-4xl text-primary mb-8 block">database</span>
                        <h4 class="text-xl font-bold mb-4 dark:text-white text-black uppercase tracking-tighter">Data
                        </h4>
                        <p class="text-sm dark:text-gray-400 text-gray-600 mb-6 leading-relaxed">Filtering signal from
                            noise. Optimizing data architecture for rapid retrieval and analytical clarity.</p>
                        <div class="flex flex-wrap gap-2">
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">Postgres</span>
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">Redis</span>
                        </div>
                    </div>
                    <div class="dark:bg-background-dark bg-white p-10 group hover:dark:bg-surface-dark transition-all">
                        <span class="material-symbols-outlined text-4xl text-primary mb-8 block">neurology</span>
                        <h4 class="text-xl font-bold mb-4 dark:text-white text-black uppercase tracking-tighter">AI</h4>
                        <p class="text-sm dark:text-gray-400 text-gray-600 mb-6 leading-relaxed">Intelligent
                            augmentation of core business logic using LLMs and predictive modeling.</p>
                        <div class="flex flex-wrap gap-2">
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">PyTorch</span>
                            <span
                                class="text-[9px] border border-border-muted px-2 py-0.5 rounded text-border-muted uppercase">OpenAI
                                SDK</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section class="py-32 px-6 dark:bg-background-dark bg-white">
            <div class="max-w-[1200px] mx-auto">
                <h2 class="text-xs font-bold text-primary uppercase tracking-[0.3em] mb-16 flex items-center gap-4">
                    <span class="w-8 h-[1px] bg-primary"></span> Selected Leverage
                </h2>
                <div class="space-y-32">
                    <div class="grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
                        <div class="space-y-8">
                            <div class="flex items-center gap-4 font-mono text-xs text-border-muted">
                                <span>[CASE_001]</span>
                                <span class="w-12 h-px bg-border-dark"></span>
                                <span>Distributed Architecture</span>
                            </div>
                            <h3 class="text-4xl font-black dark:text-white text-black tracking-tight">Financial
                                Transaction Ledger</h3>
                            <div class="space-y-6">
                                <div>
                                    <h4
                                        class="text-xs font-bold uppercase text-red-500 mb-2 tracking-widest flex items-center gap-2">
                                        <span class="material-symbols-outlined text-sm">error</span> The Problem
                                    </h4>
                                    <p class="dark:text-gray-400 text-gray-600 text-sm">Existing legacy monolith
                                        suffered from 400ms latency and 2% write-consistency errors during peak volume,
                                        stalling global settlements.</p>
                                </div>
                                <div>
                                    <h4
                                        class="text-xs font-bold uppercase text-primary mb-2 tracking-widest flex items-center gap-2">
                                        <span class="material-symbols-outlined text-sm">check_circle</span> The Leverage
                                    </h4>
                                    <p class="dark:text-gray-400 text-gray-600 text-sm">Implemented an event-driven
                                        microservices architecture using Apache Kafka for high-throughput messaging,
                                        reducing latency to &lt;15ms with 99.999% consistency.</p>
                                </div>
                            </div>
                        </div>
                        <div
                            class="relative border border-border-dark aspect-video bg-surface-dark overflow-hidden flex items-center justify-center p-8">
                            <div class="w-full h-full relative border border-primary/20 p-4">
                                <div class="absolute inset-0 opacity-20 technical-grid"></div>
                                <div class="relative flex flex-col items-center justify-center h-full space-y-4">
                                    <div
                                        class="w-24 h-24 rounded-full border-2 border-primary border-dashed flex items-center justify-center">
                                        <div class="w-12 h-12 bg-primary/20 flex items-center justify-center">
                                            <span class="material-symbols-outlined text-primary">hub</span>
                                        </div>
                                    </div>
                                    <div class="flex gap-12">
                                        <div class="w-1 h-16 bg-gradient-to-b from-primary to-transparent"></div>
                                        <div class="w-1 h-16 bg-gradient-to-b from-primary to-transparent"></div>
                                        <div class="w-1 h-16 bg-gradient-to-b from-primary to-transparent"></div>
                                    </div>
                                    <div class="grid grid-cols-3 gap-4 w-full px-8">
                                        <div class="h-8 border border-border-muted"></div>
                                        <div class="h-8 border border-border-muted"></div>
                                        <div class="h-8 border border-border-muted"></div>
                                    </div>
                                </div>
                            </div>
                            <div class="absolute bottom-4 right-4 text-[10px] font-mono text-border-muted">FIG_A:
                                DISTRIBUTED_EVENT_FLOW</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <footer class="pt-32 pb-24 px-6 dark:bg-background-dark bg-white border-t border-border-dark" id="contact">
            <div class="max-w-[1200px] mx-auto text-center space-y-12">
                <div class="space-y-4">
                    <h2
                        class="text-2xl md:text-5xl font-black dark:text-white text-black tracking-tighter leading-tight max-w-2xl mx-auto">
                        If you have a real problem worth solving, let’s talk.
                    </h2>
                </div>
                <div class="flex flex-col items-center gap-8">
                    <button
                        class="bg-primary text-background-dark px-12 py-5 text-lg font-bold uppercase tracking-widest hover:scale-105 transition-transform rounded flex items-center gap-4 group">
                        Initiate Connection
                        <span
                            class="material-symbols-outlined group-hover:translate-x-2 transition-transform">send</span>
                    </button>
                    <div
                        class="grid grid-cols-1 md:grid-cols-3 gap-12 w-full pt-16 border-t border-border-dark mt-16 text-left">
                        <div>
                            <span
                                class="text-[10px] text-border-muted font-mono uppercase block mb-4">Availability</span>
                            <p class="text-sm dark:text-gray-300 text-gray-700 font-mono">Accepting engagements for
                                Q3-Q4 2024.</p>
                        </div>
                        <div>
                            <span class="text-[10px] text-border-muted font-mono uppercase block mb-4">Focus
                                Areas</span>
                            <ul class="text-sm dark:text-gray-300 text-gray-700 space-y-1 font-mono uppercase">
                                <li>Cloud-Native Orchestration</li>
                                <li>Autonomous Agent Infrastructure</li>
                                <li>High-Performance Data Flow</li>
                            </ul>
                        </div>
                        <div class="flex flex-col justify-between">
                            <span class="text-[10px] text-border-muted font-mono uppercase block mb-4">Direct</span>
                            <div class="flex gap-4 font-mono text-xs uppercase">
                                <a class="dark:text-white text-black hover:text-primary transition-colors"
                                    href="#">LinkedIn</a>
                                <a class="dark:text-white text-black hover:text-primary transition-colors"
                                    href="#">GitHub</a>
                                <a class="dark:text-white text-black hover:text-primary transition-colors"
                                    href="#">Twitter</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </footer>
    </main>
    <div
        class="fixed bottom-0 left-0 w-full z-50 bg-[#0d0d0d] border-t border-border-dark h-12 md:h-10 flex items-center overflow-hidden font-mono text-[10px] uppercase tracking-tighter">
        <div class="max-w-[1400px] w-full mx-auto px-4 flex items-center justify-between gap-8 h-full">
            <div class="flex items-center gap-3 shrink-0">
                <div class="flex items-center gap-2">
                    <div class="relative w-2 h-2">
                        <div class="absolute inset-0 bg-system-green rounded-full pulse-soft"></div>
                        <div class="absolute inset-0 bg-system-green rounded-full scale-75"></div>
                    </div>
                    <span class="text-system-green font-bold">ONLINE</span>
                </div>
                <div class="h-3 w-px bg-border-dark"></div>
                <span class="text-gray-400">NODE:</span>
                <span class="text-white">BILLY_CRISTIAN_FAUJI.SYS</span>
            </div>
            <div class="hidden lg:flex items-center gap-2 shrink-0">
                <span class="text-gray-500">UPTIME:</span>
                <span class="text-accent-blue font-bold tabular-nums">10,432:12:45 HRS</span>
            </div>
            <div class="hidden md:flex flex-1 overflow-hidden relative">
                <div class="absolute left-0 top-0 h-full w-4 bg-gradient-to-r from-[#0d0d0d] to-transparent z-10"></div>
                <div class="ticker-scroll whitespace-nowrap flex items-center gap-12">
                    <div class="flex items-center gap-4 text-gray-500">
                        <span class="text-accent-blue">•</span> DOCKER <span class="text-accent-blue">•</span> N8N <span
                            class="text-accent-blue">•</span> POSTGRES <span class="text-accent-blue">•</span> LINUX
                        <span class="text-accent-blue">•</span> TERRAFORM <span class="text-accent-blue">•</span> KAFKA
                        <span class="text-accent-blue">•</span> KUBERNETES
                    </div>
                    <div class="flex items-center gap-4 text-gray-500">
                        <span class="text-accent-blue">•</span> DOCKER <span class="text-accent-blue">•</span> N8N <span
                            class="text-accent-blue">•</span> POSTGRES <span class="text-accent-blue">•</span> LINUX
                        <span class="text-accent-blue">•</span> TERRAFORM <span class="text-accent-blue">•</span> KAFKA
                        <span class="text-accent-blue">•</span> KUBERNETES
                    </div>
                </div>
                <div class="absolute right-0 top-0 h-full w-4 bg-gradient-to-l from-[#0d0d0d] to-transparent z-10">
                </div>
            </div>
            <div class="hidden sm:flex items-center gap-4 shrink-0">
                <div class="flex flex-col text-[8px] leading-none">
                    <span class="text-gray-600">LATENCY</span>
                    <span class="text-accent-blue">12MS</span>
                </div>
                <div class="flex items-end gap-[1px] h-4">
                    <div class="w-1 bg-border-dark h-[20%]"></div>
                    <div class="w-1 bg-border-dark h-[40%]"></div>
                    <div class="w-1 bg-accent-blue/40 h-[60%]"></div>
                    <div class="w-1 bg-accent-blue h-[30%]"></div>
                    <div class="w-1 bg-accent-blue/60 h-[80%]"></div>
                    <div class="w-1 bg-accent-blue h-[50%]"></div>
                    <div class="w-1 bg-accent-blue h-[90%]"></div>
                    <div class="w-1 bg-accent-blue h-[40%]"></div>
                </div>
            </div>
            <div class="flex items-center gap-2 shrink-0 border-l border-border-dark pl-4 ml-auto">
                <span class="text-gray-500">JKT</span>
                <span class="text-white font-bold tabular-nums">23:14:02</span>
            </div>
        </div>
    </div>
    <div class="fixed inset-0 pointer-events-none z-[-1] line-pattern opacity-10"></div>

</body>

</html>
