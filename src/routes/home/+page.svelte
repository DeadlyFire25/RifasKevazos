<svelte:head>
    <title>RifasKevazos - Rifas de Skins de Valorant</title>
    <meta name="description" content="Participa en rifas exclusivas de skins de Valorant. ¡Gana las mejores skins del juego!" />
</svelte:head>

<main class="min-h-screen bg-gradient-to-br from-slate-900 via-slate-800 to-blue-900">
    <script>
        handleLogin = () => {
            // Aquí puedes implementar la lógica de inicio de sesión
            window.location.href = '/'; // Redirige al usuario a la página de inicio de sesión
        };
    </script>
    <!-- Header -->
    <header class="relative z-10 px-6 py-4">
        <nav class="flex items-center justify-between max-w-7xl mx-auto">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 bg-gradient-to-r from-red-500 to-blue-500 rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold text-xl">RK</span>
                </div>
                <h1 class="text-2xl font-bold text-white">RifasKevazos</h1>
            </div>
            <div class="hidden md:flex items-center space-x-6">
                <a href="#rifas" class="text-gray-300 hover:text-white transition-colors">Rifas Activas</a>
                <a href="#como-participar" class="text-gray-300 hover:text-white transition-colors">Cómo Participar</a>
                <button on:click={handleLogin} class="bg-gradient-to-r from-red-500 to-pink-500 text-white px-6 py-2 rounded-lg font-semibold hover:from-red-600 hover:to-pink-600 transition-all">
                    Ingresar
                </button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="relative px-6 py-20">
        <div class="max-w-7xl mx-auto text-center">
            <div class="absolute inset-0 opacity-10">
                <div class="w-96 h-96 bg-red-500 rounded-full blur-3xl absolute top-20 left-1/4"></div>
                <div class="w-96 h-96 bg-blue-500 rounded-full blur-3xl absolute bottom-20 right-1/4"></div>
            </div>
            
            <div class="relative z-10">
                <h2 class="text-5xl md:text-7xl font-bold text-white mb-6">
                    Rifas de Skins de
                    <span class="bg-gradient-to-r from-red-400 to-blue-400 bg-clip-text text-transparent">
                        VALORANT
                    </span>
                </h2>
                <p class="text-xl text-gray-300 mb-8 max-w-3xl mx-auto">
                    Participa en rifas exclusivas y gana las mejores skins de Valorant. 
                    Desde Phantom hasta Vandal, todas las armas legendarias te esperan.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center">
                    <button class="bg-gradient-to-r from-red-500 to-pink-500 text-white px-8 py-4 rounded-xl font-bold text-lg hover:from-red-600 hover:to-pink-600 transition-all transform hover:scale-105">
                        Ver Rifas Activas
                    </button>
                    <button class="border-2 border-blue-400 text-blue-400 px-8 py-4 rounded-xl font-bold text-lg hover:bg-blue-400 hover:text-white transition-all">
                        Cómo Funciona
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Raffles -->
    <section id="rifas" class="px-6 py-16">
        <div class="max-w-7xl mx-auto">
            <h3 class="text-3xl font-bold text-white text-center mb-12">
                🎯 Rifas Destacadas
            </h3>
            
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Raffle Card 1 -->
                <div class="bg-slate-800/50 backdrop-blur-sm rounded-2xl p-6 border border-slate-700 hover:border-red-500 transition-all group">
                    <div class="aspect-video bg-gradient-to-br from-red-900 to-red-700 rounded-xl mb-4 flex items-center justify-center">
                        <span class="text-white font-bold text-xl">PHANTOM</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">Phantom Ion</h4>
                    <p class="text-gray-400 mb-4">Skin legendaria con efectos únicos</p>
                    <div class="flex justify-between items-center mb-4">
                        <span class="text-green-400 font-bold">$5.00 / Boleto</span>
                        <span class="text-gray-300">234/500 boletos</span>
                    </div>
                    <div class="bg-slate-700 rounded-full h-2 mb-4">
                        <div class="bg-gradient-to-r from-red-500 to-pink-500 h-2 rounded-full" style="width: 47%"></div>
                    </div>
                    <button class="w-full bg-gradient-to-r from-red-500 to-pink-500 text-white py-3 rounded-xl font-semibold hover:from-red-600 hover:to-pink-600 transition-all">
                        Participar Ahora
                    </button>
                </div>

                <!-- Raffle Card 2 -->
                <div class="bg-slate-800/50 backdrop-blur-sm rounded-2xl p-6 border border-slate-700 hover:border-blue-500 transition-all group">
                    <div class="aspect-video bg-gradient-to-br from-blue-900 to-blue-700 rounded-xl mb-4 flex items-center justify-center">
                        <span class="text-white font-bold text-xl">VANDAL</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">Vandal Reaver</h4>
                    <p class="text-gray-400 mb-4">Diseño oscuro y elegante</p>
                    <div class="flex justify-between items-center mb-4">
                        <span class="text-green-400 font-bold">$7.50 / Boleto</span>
                        <span class="text-gray-300">89/300 boletos</span>
                    </div>
                    <div class="bg-slate-700 rounded-full h-2 mb-4">
                        <div class="bg-gradient-to-r from-blue-500 to-cyan-500 h-2 rounded-full" style="width: 30%"></div>
                    </div>
                    <button class="w-full bg-gradient-to-r from-blue-500 to-cyan-500 text-white py-3 rounded-xl font-semibold hover:from-blue-600 hover:to-cyan-600 transition-all">
                        Participar Ahora
                    </button>
                </div>

                <!-- Raffle Card 3 -->
                <div class="bg-slate-800/50 backdrop-blur-sm rounded-2xl p-6 border border-slate-700 hover:border-purple-500 transition-all group">
                    <div class="aspect-video bg-gradient-to-br from-purple-900 to-purple-700 rounded-xl mb-4 flex items-center justify-center">
                        <span class="text-white font-bold text-xl">OPERATOR</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">Operator Dragon</h4>
                    <p class="text-gray-400 mb-4">Skin épica con animaciones</p>
                    <div class="flex justify-between items-center mb-4">
                        <span class="text-green-400 font-bold">$10.00 / Boleto</span>
                        <span class="text-gray-300">156/200 boletos</span>
                    </div>
                    <div class="bg-slate-700 rounded-full h-2 mb-4">
                        <div class="bg-gradient-to-r from-purple-500 to-pink-500 h-2 rounded-full" style="width: 78%"></div>
                    </div>
                    <button class="w-full bg-gradient-to-r from-purple-500 to-pink-500 text-white py-3 rounded-xl font-semibold hover:from-purple-600 hover:to-pink-600 transition-all">
                        Participar Ahora
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- How it Works -->
    <section id="como-participar" class="px-6 py-16 bg-slate-800/30">
        <div class="max-w-7xl mx-auto">
            <h3 class="text-3xl font-bold text-white text-center mb-12">
                ⚡ Cómo Participar
            </h3>
            
            <div class="grid md:grid-cols-3 gap-8">
                <div class="text-center">
                    <div class="w-16 h-16 bg-gradient-to-r from-red-500 to-pink-500 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-white font-bold text-2xl">1</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">Elige tu Rifa</h4>
                    <p class="text-gray-400">Selecciona la skin que más te guste de nuestras rifas activas</p>
                </div>
                
                <div class="text-center">
                    <div class="w-16 h-16 bg-gradient-to-r from-blue-500 to-cyan-500 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-white font-bold text-2xl">2</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">Compra Boletos</h4>
                    <p class="text-gray-400">Adquiere tus boletos de forma segura y rápida</p>
                </div>
                
                <div class="text-center">
                    <div class="w-16 h-16 bg-gradient-to-r from-purple-500 to-pink-500 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-white font-bold text-2xl">3</span>
                    </div>
                    <h4 class="text-white font-bold text-xl mb-2">¡Gana!</h4>
                    <p class="text-gray-400">Espera el sorteo y recibe tu skin directamente en tu cuenta</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Stats -->
    <section class="px-6 py-16">
        <div class="max-w-7xl mx-auto">
            <div class="grid md:grid-cols-4 gap-8 text-center">
                <div>
                    <div class="text-4xl font-bold text-white mb-2">1,250+</div>
                    <div class="text-gray-400">Skins Entregadas</div>
                </div>
                <div>
                    <div class="text-4xl font-bold text-white mb-2">5,680+</div>
                    <div class="text-gray-400">Usuarios Felices</div>
                </div>
                <div>
                    <div class="text-4xl font-bold text-white mb-2">24/7</div>
                    <div class="text-gray-400">Soporte</div>
                </div>
                <div>
                    <div class="text-4xl font-bold text-white mb-2">100%</div>
                    <div class="text-gray-400">Seguro</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="px-6 py-12 border-t border-slate-700">
        <div class="max-w-7xl mx-auto text-center">
            <div class="flex items-center justify-center space-x-3 mb-4">
                <div class="w-8 h-8 bg-gradient-to-r from-red-500 to-blue-500 rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold">RK</span>
                </div>
                <span class="text-white font-bold text-xl">RifasKevazos</span>
            </div>
            <p class="text-gray-400 mb-4">
                La plataforma más confiable para rifas de skins de Valorant
            </p>
            <div class="flex justify-center space-x-6 text-gray-400">
                <a href="/" class="hover:text-white transition-colors">Términos</a>
                <a href="/" class="hover:text-white transition-colors">Privacidad</a>
                <a href="/" class="hover:text-white transition-colors">Contacto</a>
                <a href="/" class="hover:text-white transition-colors">Discord</a>
            </div>
        </div>
    </footer>
</main>

<style>
    :global(body) {
        margin: 0;
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    }
    
    @keyframes pulse {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.7; }
    }
    
    .group:hover .animate-pulse {
        animation: pulse 2s infinite;
    }
</style>