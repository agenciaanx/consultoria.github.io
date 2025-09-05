<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Agência ANX - Marketing Digital e Performance</title>
    <!-- Fonte "Inter" do Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --bg-light: #F5F5F5;
            --text-dark: #1A1A1A;
            --text-muted: #6B7280;
            --accent-gray: #D1D5DB;
            --card-light: #E5E7EB;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
        }

        .whatsapp-icon {
            width: 24px;
            height: 24px;
            fill: currentColor;
        }

        /* Animação de entrada ao rolar */
        .hidden-section {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }

        .visible-section {
            opacity: 1;
            transform: translateY(0);
        }

        /* Animação para o botão de CTA (pulso) */
        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
        }
        .animate-pulse-cta {
            animation: pulse 2s infinite ease-in-out;
        }
    </style>
</head>
<body class="bg-white text-zinc-950 min-h-screen flex flex-col">

    <!-- Cabeçalho (Header) com apenas o logotipo -->
    <header class="sticky top-0 bg-white/90 backdrop-blur-sm z-50 py-4 px-4 md:px-8 border-b border-gray-300">
        <div class="container mx-auto flex justify-center items-center">
            <!-- Logotipo -->
            <a href="#" class="text-3xl font-extrabold text-zinc-950 tracking-tight">ANX<span class="text-gray-600">.</span></a>
        </div>
    </header>

    <main class="flex-grow">
        <!-- Secção Principal (Hero) -->
        <section id="hero" class="py-20 md:py-32 px-4 text-center">
            <div class="container mx-auto max-w-4xl">
                <p class="text-sm font-semibold text-gray-600 mb-4">A sua agência de marketing</p>
                <h1 class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-extrabold leading-tight mb-6 text-zinc-950">
                    <span class="block">Seu negócio na internet</span>
                    <span class="block text-gray-600">com resultados reais.</span>
                </h1>
                <p class="text-base md:text-lg text-gray-500 mb-8">
                    Analisamos, planejamos e executamos a estratégia de marketing digital ideal para sua empresa.
                </p>
                <a href="https://api.whatsapp.com/send?phone=5521997262954&text=Quero+agendar+a+consultoria+especializada" target="_blank" class="inline-flex items-center justify-center space-x-2 bg-gray-900 hover:bg-gray-800 text-white font-bold py-3 px-8 rounded-full shadow-lg transform transition-transform duration-300 ease-in-out animate-pulse-cta focus:outline-none focus:ring-4 focus:ring-gray-300">
                    <svg class="whatsapp-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
                        <path d="M380.9 97.1C339.4 56.5 285.8 32 227.4 32h-1.4C108.6 32 15.6 112.5 15.6 220c0 31.6 8.5 62.6 24.5 90.5L8.5 450.7c-2.3 8.8 4.2 17.5 13.5 17.5h.3l98.3-25.5c26.2 15.6 56.4 23.5 87.2 23.5h1.4c118.8 0 211.8-80.5 211.8-188.5 0-48.4-18.4-93.5-51.3-127.9zM227.4 457.1c-29.3 0-57.9-7.9-82.5-23.5l-6.4-4.8L61.7 445l16.2-59.5-3.8-6.1c-15.3-24.8-23.5-53.7-23.5-84.3 0-97.1 82.5-176.4 184.2-176.4h1.4c89.7 0 162.7 73.1 162.7 170.2s-73 170.2-162.7 170.2zM337 266.8c-2.6-1.3-15.3-7.5-17.6-8.3-2.3-.8-4.7-1.3-6.8 1.3-2.1 2.6-8 1.3-9.8.7-1.8-.7-4.2-1.3-6.8-2.6-2.6-1.3-2.6-2.6-4.2-4.2-1.6-1.6-3.8-3.3-5.2-4.9-1.4-1.6-2.6-1.3-4.2-2.6-1.6-1.3-3.3-2.6-4.9-3.9-1.6-1.3-3.3-1.8-5.7-1.3-2.3.6-4.7 2.6-6.4 4.2-1.6 1.6-4.2 4.9-4.2 11.2 0 6.3 4.2 12.5 5.2 13.5 1 1 9.8 17.6 12.5 20.3 2.6 2.6 4.9 3.9 8.2 3.9 3.3 0 5.2-.2 9.8-.7s17.6-7.3 20.3-9.8c2.6-2.6 4.9-4.2 4.9-6.8 0-2.6-1.8-4.2-3.3-5.5z"/>
                    </svg>
                    <span>Falar com um especialista</span>
                </a>
            </div>
        </section>
        
        <!-- Secção de Soluções/Serviços -->
        <section id="solucoes" class="py-16 px-4 bg-gray-100 hidden-section rounded-3xl">
            <div class="container mx-auto max-w-6xl">
                <div class="text-center mb-12">
                    <p class="text-sm font-semibold text-gray-600 mb-2">SOLUÇÕES</p>
                    <h2 class="text-3xl md:text-4xl font-extrabold text-zinc-950">O que fazemos</h2>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Card 1 -->
                    <div class="bg-white p-8 rounded-2xl border border-gray-300 shadow-xl hidden-section">
                        <div class="text-4xl text-gray-600 mb-4">
                            <span class="inline-block p-3 rounded-full bg-gray-300">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                                </svg>
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-2 text-zinc-950">Análise de Dados</h3>
                        <p class="text-gray-500">
                            Tomamos decisões inteligentes com base em dados para maximizar o seu ROI e garantir o crescimento do seu negócio.
                        </p>
                    </div>
                    <!-- Card 2 -->
                    <div class="bg-white p-8 rounded-2xl border border-gray-300 shadow-xl hidden-section">
                        <div class="text-4xl text-gray-600 mb-4">
                            <span class="inline-block p-3 rounded-full bg-gray-300">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 12l3-3 3 3 4-4M18 14V6m0 0l-4 4m4-4l4 4" />
                                </svg>
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-2 text-zinc-950">Tráfego Pago</h3>
                        <p class="text-gray-500">
                            Criamos e gerenciamos campanhas de publicidade para atrair clientes qualificados para sua empresa.
                        </p>
                    </div>
                    <!-- Card 3 -->
                    <div class="bg-white p-8 rounded-2xl border border-gray-300 shadow-xl hidden-section">
                        <div class="text-4xl text-gray-600 mb-4">
                            <span class="inline-block p-3 rounded-full bg-gray-300">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 10V3L4 14h7v7l9-11h-7z" />
                                </svg>
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-2 text-zinc-950">Otimização de Jornada do Cliente</h3>
                        <p class="text-gray-500">
                            Analisamos e otimizamos a jornada do cliente, transformando visitantes em compradores fiéis.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Secção de Clientes/Portfólio -->
        <section id="clientes" class="py-16 px-4 bg-white hidden-section">
            <div class="container mx-auto max-w-6xl">
                <div class="text-center mb-12">
                    <p class="text-sm font-semibold text-gray-600 mb-2">PORTFÓLIO</p>
                    <h2 class="text-3xl md:text-4xl font-extrabold text-zinc-950">Casos de sucesso</h2>
                </div>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Case 1 -->
                    <div class="rounded-xl overflow-hidden shadow-lg hidden-section">
                        <img src="https://placehold.co/600x400/E5E7EB/6B7280?text=E-commerce" alt="Capa de projeto de e-commerce" class="w-full h-auto object-cover">
                        <div class="p-6 bg-gray-200">
                            <h3 class="text-xl font-bold text-zinc-950 mb-1">E-commerce de Roupas</h3>
                            <p class="text-gray-500 text-sm">Aumento de 200% em vendas online.</p>
                        </div>
                    </div>
                    <!-- Case 2 -->
                    <div class="rounded-xl overflow-hidden shadow-lg hidden-section">
                        <img src="https://placehold.co/600x400/E5E7EB/6B7280?text=Consultoria" alt="Capa de projeto de consultoria" class="w-full h-auto object-cover">
                        <div class="p-6 bg-gray-200">
                            <h3 class="text-xl font-bold text-zinc-950 mb-1">Consultoria Financeira</h3>
                            <p class="text-gray-500 text-sm">Redução de 30% no custo por lead.</p>
                        </div>
                    </div>
                    <!-- Case 3 -->
                    <div class="rounded-xl overflow-hidden shadow-lg hidden-section">
                        <img src="https://placehold.co/600x400/E5E7EB/6B7280?text=Tecnologia" alt="Capa de projeto de tecnologia" class="w-full h-auto object-cover">
                        <div class="p-6 bg-gray-200">
                            <h3 class="text-xl font-bold text-zinc-950 mb-1">Startup de Tecnologia</h3>
                            <p class="text-gray-500 text-sm">Crescimento de 50% no tráfego orgânico.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Secção de Depoimentos -->
        <section id="depoimentos" class="py-16 px-4 bg-gray-100 hidden-section rounded-3xl">
            <div class="container mx-auto max-w-4xl text-center">
                <blockquote class="text-2xl md:text-3xl font-light italic text-gray-600 mb-6">
                    "O trabalho da Agência ANX é impecável. Nossa equipe viu um aumento substancial de clientes e de receitas graças à estratégia de tráfego pago."
                </blockquote>
                <p class="font-semibold text-lg text-gray-500">
                    — André M., Diretor Comercial
                </p>
            </div>
        </section>

        <!-- Secção Final de CTA (Contato) -->
        <section id="contato" class="py-16 md:py-24 px-4 bg-gray-100 text-zinc-950 rounded-3xl hidden-section">
            <div class="container mx-auto max-w-4xl text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-4 text-zinc-950">
                    Pronto para decolar?
                </h2>
                <p class="text-lg md:text-xl mb-8 max-w-2xl mx-auto opacity-90 text-gray-500">
                    Vamos falar sobre o futuro do seu negócio.
                </p>
                <!-- Botão de CTA para WhatsApp -->
                <a href="https://api.whatsapp.com/send?phone=5521997262954&text=Quero+agendar+a+consultoria+especializada" target="_blank" class="inline-flex items-center justify-center space-x-2 bg-gray-900 hover:bg-gray-800 text-white font-bold py-3 px-8 rounded-full shadow-lg transform transition-transform duration-300 ease-in-out animate-pulse-cta focus:outline-none focus:ring-4 focus:ring-gray-300">
                    <svg class="whatsapp-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
                        <path d="M380.9 97.1C339.4 56.5 285.8 32 227.4 32h-1.4C108.6 32 15.6 112.5 15.6 220c0 31.6 8.5 62.6 24.5 90.5L8.5 450.7c-2.3 8.8 4.2 17.5 13.5 17.5h.3l98.3-25.5c26.2 15.6 56.4 23.5 87.2 23.5h1.4c118.8 0 211.8-80.5 211.8-188.5 0-48.4-18.4-93.5-51.3-127.9zM227.4 457.1c-29.3 0-57.9-7.9-82.5-23.5l-6.4-4.8L61.7 445l16.2-59.5-3.8-6.1c-15.3-24.8-23.5-53.7-23.5-84.3 0-97.1 82.5-176.4 184.2-176.4h1.4c89.7 0 162.7 73.1 162.7 170.2s-73 170.2-162.7 170.2zM337 266.8c-2.6-1.3-15.3-7.5-17.6-8.3-2.3-.8-4.7-1.3-6.8 1.3-2.1 2.6-8 1.3-9.8.7-1.8-.7-4.2-1.3-6.8-2.6-2.6-1.3-2.6-2.6-4.2-4.2-1.6-1.6-3.8-3.3-5.2-4.9-1.4-1.6-2.6-1.3-4.2-2.6-1.6-1.3-3.3-2.6-4.9-3.9-1.6-1.3-3.3-1.8-5.7-1.3-2.3.6-4.7 2.6-6.4 4.2-1.6 1.6-4.2 4.9-4.2 11.2 0 6.3 4.2 12.5 5.2 13.5 1 1 9.8 17.6 12.5 20.3 2.6 2.6 4.9 3.9 8.2 3.9 3.3 0 5.2-.2 9.8-.7s17.6-7.3 20.3-9.8c2.6-2.6 4.9-4.2 4.9-6.8 0-2.6-1.8-4.2-3.3-5.5z"/>
                    </svg>
                    <span>Fale conosco</span>
                </a>
            </div>
        </section>
    </main>

    <!-- Rodapé -->
    <footer class="bg-white text-zinc-950 py-8 text-center border-t border-gray-300">
        <div class="container mx-auto px-4">
            <p class="text-sm text-gray-500">
                &copy; 2024 Agência ANX. Todos os direitos reservados.
            </p>
        </div>
    </footer>

    <!-- Scripts -->
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            // Observer para animações de entrada das secções
            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible-section');
                        entry.target.classList.remove('hidden-section');
                        // Deixa de observar depois de animar
                        observer.unobserve(entry.target); 
                    }
                });
            }, {
                // Porcentagem do elemento que precisa estar visível para disparar a animação
                threshold: 0.1 
            });

            // Adiciona as secções para o observador
            const sections = document.querySelectorAll('.hidden-section');
            sections.forEach(section => {
                observer.observe(section);
            });
        });
    </script>
</body>
</html>
