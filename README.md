<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pet Blue | Pet Sitter, Pet Hostel e Day Care em Extrema - MG</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts Inter e Outfit -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Outfit:wght@500;600;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0f7ff',
                            100: '#e0effe',
                            200: '#bae0fd',
                            500: '#0084ff',
                            600: '#0066cc',
                            700: '#004da3',
                            800: '#003575',
                            900: '#00224d',
                        },
                        navy: {
                            800: '#0f172a',
                            900: '#090d16',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Outfit', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .gradient-text {
            background: linear-gradient(135deg, #0084ff 0%, #004da3 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .hero-bg {
            background: radial-gradient(circle at top right, rgba(0, 132, 255, 0.12), transparent 40%),
                        radial-gradient(circle at bottom left, rgba(0, 77, 163, 0.08), transparent 40%);
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(224, 239, 254, 0.8);
        }
    </style>
</head>
<body class="font-sans text-slate-700 bg-slate-50 antialiased selection:bg-brand-500 selection:text-white">

    <!-- BARRA SUPERIOR DE INFORMAÇÕES RÁPIDAS -->
    <div class="bg-brand-900 text-slate-300 text-xs sm:text-sm py-2 px-4 border-b border-brand-800">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-2">
            <div class="flex items-center space-x-4">
                <span class="flex items-center gap-1.5"><i class="fa-solid font-bold fa-location-dot text-brand-500"></i> Rua São Paulo, 150, Centro - Extrema/MG</span>
                <span class="hidden md:flex items-center gap-1.5"><i class="fa-regular fa-clock text-brand-500"></i> Seg - Sex: 08h às 18h | Sáb: 08h às 12h</span>
            </div>
            <div class="flex items-center space-x-4">
                <a href="https://instagram.com/petblue_extrema" target="_blank" class="hover:text-brand-200 transition-colors flex items-center gap-1">
                    <i class="fa-brands fa-instagram text-brand-500"></i> @petblue_extrema
                </a>
                <span class="hidden sm:inline text-slate-600">|</span>
                <a href="mailto:petblue2026@gmail.com" class="hover:text-brand-200 transition-colors flex items-center gap-1">
                    <i class="fa-regular fa-envelope text-brand-500"></i> petblue2026@gmail.com
                </a>
            </div>
        </div>
    </div>

    <!-- CABEÇALHO E NAVEGAÇÃO -->
    <header class="sticky top-0 z-40 bg-white/90 backdrop-blur-md shadow-sm border-b border-slate-100 transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- LOGO -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-12 h-12 rounded-2xl bg-gradient-to-tr from-brand-700 to-brand-500 flex items-center justify-center text-white shadow-lg shadow-brand-500/30 group-hover:scale-105 transition-transform duration-300">
                    <i class="fa-solid fa-paw text-2xl"></i>
                </div>
                <div class="flex flex-col">
                    <span class="font-display font-extrabold text-2xl tracking-tight text-slate-900 leading-none">Pet<span class="text-brand-600">Blue</span></span>
                    <span class="text-[10px] font-semibold text-slate-400 tracking-wider uppercase mt-1">Care & Comfort</span>
                </div>
            </a>

            <!-- NAV DESKTOP -->
            <nav class="hidden lg:flex items-center space-x-8 font-medium text-slate-600 text-sm">
                <a href="#inicio" class="hover:text-brand-600 transition-colors">Início</a>
                <a href="#sobre" class="hover:text-brand-600 transition-colors">Sobre Nós</a>
                <a href="#servicos" class="hover:text-brand-600 transition-colors">Serviços</a>
                <a href="#diferenciais" class="hover:text-brand-600 transition-colors">Diferenciais</a>
                <a href="#horarios" class="hover:text-brand-600 transition-colors">Horários</a>
                <a href="#contato" class="hover:text-brand-600 transition-colors">Localização</a>
            </nav>

            <!-- CTA WHATSAPP BOTÃO -->
            <div class="hidden sm:flex items-center gap-3">
                <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20gostaria%20de%20informa%C3%A7%C3%B5es%20sobre%20os%20servi%C3%A7os%20do%20Pet%20Blue." 
                   target="_blank"
                   class="bg-emerald-500 hover:bg-emerald-600 text-white font-semibold text-sm px-5 py-2.5 rounded-full shadow-lg shadow-emerald-500/25 flex items-center gap-2 transition-all duration-300 transform hover:-translate-y-0.5">
                    <i class="fa-brands fa-whatsapp text-lg"></i>
                    <span>Falar no WhatsApp</span>
                </a>
            </div>

            <!-- BOTÃO MOBILE MENU -->
            <button id="mobile-menu-btn" class="lg:hidden p-2 rounded-xl text-slate-600 hover:text-brand-600 hover:bg-slate-100 transition-colors">
                <i class="fa-solid fa-bars text-2xl"></i>
            </button>
        </div>

        <!-- MENU MOBILE DROPDOWN -->
        <div id="mobile-menu" class="hidden lg:hidden bg-white border-b border-slate-200 px-6 py-6 space-y-4">
            <a href="#inicio" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Início</a>
            <a href="#sobre" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Sobre Nós</a>
            <a href="#servicos" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Serviços</a>
            <a href="#diferenciais" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Diferenciais</a>
            <a href="#horarios" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Horários</a>
            <a href="#contato" class="mobile-link block text-slate-700 hover:text-brand-600 font-medium py-1">Localização</a>
            <div class="pt-4 border-t border-slate-100">
                <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20gostaria%20de%20informa%C3%A7%C3%B5es%20sobre%20os%20servi%C3%A7os%20do%20Pet%20Blue." 
                   target="_blank"
                   class="w-full bg-emerald-500 hover:bg-emerald-600 text-white font-semibold text-center py-3 rounded-xl flex items-center justify-center gap-2 shadow-md">
                    <i class="fa-brands fa-whatsapp text-lg"></i>
                    <span>Conversar no WhatsApp</span>
                </a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section id="inicio" class="hero-bg relative overflow-hidden py-16 lg:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- TEXTO HERO -->
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-brand-50 border border-brand-200 text-brand-700 text-xs sm:text-sm font-semibold tracking-wide">
                        <i class="fa-solid fa-heart text-brand-500"></i>
                        <span>Desde 2021 oferecendo experiências únicas em Extrema</span>
                    </div>

                    <h1 class="font-display font-extrabold text-4xl sm:text-5xl lg:text-6xl text-slate-900 leading-[1.15]">
                        VOCÊ E SEU PET <span class="gradient-text">TRANQUILOS!</span>
                    </h1>

                    <p class="text-lg sm:text-xl text-slate-600 max-w-2xl mx-auto lg:mx-0 font-light leading-relaxed">
                        Seu pet em boas mãos em Extrema - MG. Cuidado amoroso, hospedagem aconchegante, creche diária e acompanhamento individualizado.
                    </p>

                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
                        <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Quero%20agendar%20um%20servi%C3%A7o%20para%20o%20meu%20pet." 
                           target="_blank" 
                           class="w-full sm:w-auto bg-brand-600 hover:bg-brand-700 text-white font-bold text-base px-8 py-4 rounded-2xl shadow-lg shadow-brand-600/30 flex items-center justify-center gap-3 transition-all transform hover:-translate-y-1">
                            <i class="fa-brands fa-whatsapp text-xl"></i>
                            <span>Falar no WhatsApp</span>
                        </a>

                        <a href="#servicos" 
                           class="w-full sm:w-auto bg-white hover:bg-slate-100 text-slate-700 border border-slate-200 font-semibold text-base px-8 py-4 rounded-2xl flex items-center justify-center gap-2 transition-colors">
                            <span>Conhecer Serviços</span>
                            <i class="fa-solid fa-arrow-down text-xs"></i>
                        </a>
                    </div>

                    <!-- SELOS DE CONFIANÇA -->
                    <div class="pt-8 grid grid-cols-3 gap-4 border-t border-slate-200/80 max-w-lg mx-auto lg:mx-0">
                        <div class="text-center lg:text-left">
                            <span class="block font-display font-extrabold text-2xl text-slate-900">Desde 2021</span>
                            <span class="text-xs text-slate-500 font-medium">Tradição & Cuidado</span>
                        </div>
                        <div class="text-center lg:text-left">
                            <span class="block font-display font-extrabold text-2xl text-slate-900">100%</span>
                            <span class="text-xs text-slate-500 font-medium">Amor & Dedicação</span>
                        </div>
                        <div class="text-center lg:text-left">
                            <span class="block font-display font-extrabold text-2xl text-slate-900">Extrema/MG</span>
                            <span class="text-xs text-slate-500 font-medium">Localização Central</span>
                        </div>
                    </div>
                </div>

                <!-- CARD ILUSTRATIVO SEM IMAGENS -->
                <div class="lg:col-span-5 relative">
                    <div class="relative mx-auto max-w-md lg:max-w-none">
                        <div class="bg-gradient-to-br from-brand-600 to-brand-800 rounded-3xl p-8 text-white shadow-2xl relative overflow-hidden">
                            <div class="absolute -right-10 -bottom-10 opacity-10 text-white text-9xl">
                                <i class="fa-solid fa-paw"></i>
                            </div>

                            <div class="space-y-6 relative z-10">
                                <div class="w-16 h-16 rounded-2xl bg-white/10 backdrop-blur-md flex items-center justify-center text-3xl border border-white/20">
                                    <i class="fa-solid fa-house-chimney-window"></i>
                                </div>

                                <h3 class="font-display font-bold text-2xl">Estrutura Pensada no Bem-Estar</h3>
                                <p class="text-brand-100 text-sm leading-relaxed">
                                    Segurança, diversão e acompanhamento carinhoso em cada momento do dia do seu animalzinho.
                                </p>

                                <div class="space-y-3 pt-2 border-t border-white/10">
                                    <div class="flex items-center gap-3 text-sm">
                                        <i class="fa-solid fa-bone text-brand-200"></i>
                                        <span>Pet Sitter na sua residência</span>
                                    </div>
                                    <div class="flex items-center gap-3 text-sm">
                                        <i class="fa-solid fa-hotel text-brand-200"></i>
                                        <span>Hospedagem tranquila (Pet Hostel)</span>
                                    </div>
                                    <div class="flex items-center gap-3 text-sm">
                                        <i class="fa-solid fa-sun text-brand-200"></i>
                                        <span>Creche e brincadeiras (Day Care)</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SOBRE NÓS -->
    <section id="sobre" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                
                <div class="space-y-6">
                    <div class="inline-block px-3 py-1 rounded-md bg-brand-100 text-brand-700 text-xs font-bold uppercase tracking-wider">Sobre o Pet Blue</div>
                    <h2 class="font-display font-extrabold text-3xl sm:text-4xl text-slate-900">
                        O refúgio perfeito para o seu pet enquanto você cumpre seus compromissos
                    </h2>
                    <p class="text-slate-600 leading-relaxed">
                        No <strong>Pet Blue</strong>, entendemos que seu pet é parte da sua família. Por isso, desde 2021 nos dedicamos a criar um ambiente acolhedor, seguro e divertido em Extrema - MG.
                    </p>
                    <p class="text-slate-600 leading-relaxed">
                        Seja para passar o dia na nossa creche (Day Care), ter uma hospedagem aconchegante no Pet Hostel ou receber cuidados personalizados com o Pet Sitter, nossa equipe é dedicada em tempo integral ao bem-estar animal.
                    </p>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                    <div class="bg-brand-50 p-6 rounded-3xl border border-brand-100 space-y-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 text-white flex items-center justify-center font-bold">
                            <i class="fa-solid fa-shield-heart"></i>
                        </div>
                        <h4 class="font-bold text-slate-900">Segurança Total</h4>
                        <p class="text-xs text-slate-600">Ambiente monitorado e protegido para a total tranquilidade do tutor.</p>
                    </div>

                    <div class="bg-brand-50 p-6 rounded-3xl border border-brand-100 space-y-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 text-white flex items-center justify-center font-bold">
                            <i class="fa-solid fa-face-smile-beam"></i>
                        </div>
                        <h4 class="font-bold text-slate-900">Socialização</h4>
                        <p class="text-xs text-slate-600">Atividades e rotinas dinâmicas para seu pet fazer novos amigos.</p>
                    </div>

                    <div class="bg-brand-50 p-6 rounded-3xl border border-brand-100 space-y-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 text-white flex items-center justify-center font-bold">
                            <i class="fa-solid fa-comments"></i>
                        </div>
                        <h4 class="font-bold text-slate-900">Notícias Diárias</h4>
                        <p class="text-xs text-slate-600">Comunicação constante via WhatsApp durante toda a estadia.</p>
                    </div>

                    <div class="bg-brand-50 p-6 rounded-3xl border border-brand-100 space-y-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 text-white flex items-center justify-center font-bold">
                            <i class="fa-solid fa-map-pin"></i>
                        </div>
                        <h4 class="font-bold text-slate-900">Fácil Acesso</h4>
                        <p class="text-xs text-slate-600">Localização bem no Centro de Extrema para sua maior comodidade.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SERVIÇOS -->
    <section id="servicos" class="py-20 bg-slate-100/70 relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-4">
                <span class="px-3.5 py-1.5 rounded-full bg-brand-100 text-brand-700 text-xs font-bold uppercase tracking-wider">Nossos Serviços Especializados</span>
                <h2 class="font-display font-extrabold text-3xl sm:text-4xl text-slate-900">
                    Tudo o que seu Pet precisa para ser feliz
                </h2>
                <p class="text-slate-600">
                    Modalidades sob medida para atender a rotina da sua família com carinho e profissionalismo.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                
                <!-- CARD SERVIÇO 1 -->
                <div class="bg-white rounded-3xl p-8 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 flex flex-col justify-between group">
                    <div>
                        <div class="w-16 h-16 rounded-2xl bg-brand-50 text-brand-600 flex items-center justify-center text-3xl mb-6 group-hover:bg-brand-600 group-hover:text-white transition-colors duration-300 shadow-md">
                            <i class="fa-solid fa-user-nurse"></i>
                        </div>
                        <h3 class="font-display font-bold text-2xl text-slate-900 mb-3">Pet Sitter</h3>
                        <p class="text-slate-600 text-sm leading-relaxed mb-6">
                            Cuidados personalizados e atenção no aconchego do lar. Ideal para animais que preferem sua própria rotina de passeios e alimentação.
                        </p>
                        <ul class="space-y-2.5 text-xs text-slate-500 font-medium border-t border-slate-100 pt-4 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Alimentação & Troca de Água</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Higienização do Espaço</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Passeios e Companhia</li>
                        </ul>
                    </div>
                    <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Gostaria%20de%20saber%20mais%20sobre%20o%20servi%C3%A7o%20de%20Pet%20Sitter." 
                       target="_blank" 
                       class="w-full bg-slate-50 group-hover:bg-brand-600 text-slate-700 group-hover:text-white font-semibold py-3 px-4 rounded-xl text-center text-sm transition-colors duration-300 block">
                        Consultar Pet Sitter
                    </a>
                </div>

                <!-- CARD SERVIÇO 2 (DESTAQUE) -->
                <div class="bg-gradient-to-b from-brand-900 to-slate-900 text-white rounded-3xl p-8 shadow-xl transition-all duration-300 flex flex-col justify-between transform lg:-translate-y-2 relative overflow-hidden">
                    <div class="absolute top-4 right-4 bg-brand-500 text-white text-[10px] font-bold px-3 py-1 rounded-full uppercase tracking-wider">
                        Mais Procurado
                    </div>
                    <div>
                        <div class="w-16 h-16 rounded-2xl bg-brand-500 text-white flex items-center justify-center text-3xl mb-6 shadow-lg shadow-brand-500/40">
                            <i class="fa-solid fa-hotel"></i>
                        </div>
                        <h3 class="font-display font-bold text-2xl text-white mb-3">Pet Hostel</h3>
                        <p class="text-slate-300 text-sm leading-relaxed mb-6">
                            Vai viajar? Hospedagem acolhedora, segura e sem estresse para seu amigo dormir bem e se divertir com total acompanhamento.
                        </p>
                        <ul class="space-y-2.5 text-xs text-slate-300 font-medium border-t border-slate-800 pt-4 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-emerald-400"></i> Pernoite Monitorado</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-emerald-400"></i> Envio Diário de Notícias</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-emerald-400"></i> Ambientes Confortáveis</li>
                        </ul>
                    </div>
                    <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Gostaria%20de%20reservar%20uma%20vaga%20no%20Pet%20Hostel." 
                       target="_blank" 
                       class="w-full bg-brand-500 hover:bg-brand-600 text-white font-semibold py-3.5 px-4 rounded-xl text-center text-sm shadow-md transition-colors block">
                        Reservar Hospedagem
                    </a>
                </div>

                <!-- CARD SERVIÇO 3 -->
                <div class="bg-white rounded-3xl p-8 shadow-sm hover:shadow-xl transition-all duration-300 border border-slate-200/80 flex flex-col justify-between group">
                    <div>
                        <div class="w-16 h-16 rounded-2xl bg-brand-50 text-brand-600 flex items-center justify-center text-3xl mb-6 group-hover:bg-brand-600 group-hover:text-white transition-colors duration-300 shadow-md">
                            <i class="fa-solid fa-sun"></i>
                        </div>
                        <h3 class="font-display font-bold text-2xl text-slate-900 mb-3">Day Care</h3>
                        <p class="text-slate-600 text-sm leading-relaxed mb-6">
                            A creche perfeita para quem trabalha fora. O pet gasta energia de forma saudável, melhora o comportamento e não fica sozinho.
                        </p>
                        <ul class="space-y-2.5 text-xs text-slate-500 font-medium border-t border-slate-100 pt-4 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Socialização Orientada</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Atividades Recreativas</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-circle-check text-brand-500"></i> Redução do Estresse</li>
                        </ul>
                    </div>
                    <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Gostaria%20de%20informa%C3%A7%C3%B5es%20sobre%20o%20Day%20Care%20(Creche)." 
                       target="_blank" 
                       class="w-full bg-slate-50 group-hover:bg-brand-600 text-slate-700 group-hover:text-white font-semibold py-3 px-4 rounded-xl text-center text-sm transition-colors duration-300 block">
                        Matricular no Day Care
                    </a>
                </div>

            </div>
        </div>
    </section>

    <!-- HORÁRIOS DE FUNCIONAMENTO -->
    <section id="horarios" class="py-20 bg-slate-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-6 space-y-6">
                    <span class="px-3.5 py-1.5 rounded-full bg-brand-500/20 text-brand-300 border border-brand-500/30 text-xs font-bold uppercase tracking-wider">Disponibilidade</span>
                    <h2 class="font-display font-extrabold text-3xl sm:text-4xl text-white">
                        Horários de Atendimento
                    </h2>
                    <p class="text-slate-400 leading-relaxed">
                        Estamos abertos nos melhores horários da semana para facilitar a sua rotina no Centro de Extrema - MG.
                    </p>

                    <div class="flex items-center gap-4 p-4 rounded-2xl bg-slate-800/80 border border-slate-700">
                        <div class="w-10 h-10 rounded-full bg-emerald-500/20 text-emerald-400 flex items-center justify-center text-lg">
                            <i class="fa-solid fa-circle-check"></i>
                        </div>
                        <div>
                            <span class="block text-sm font-bold text-white">Dúvidas sobre horários especiais?</span>
                            <span class="text-xs text-slate-400">Entre em contato no WhatsApp para organizar check-in do Hostel.</span>
                        </div>
                    </div>
                </div>

                <!-- CARD HORÁRIOS -->
                <div class="lg:col-span-6">
                    <div class="bg-slate-800 rounded-3xl p-6 sm:p-8 border border-slate-700 shadow-2xl space-y-4">
                        <div class="flex items-center justify-between border-b border-slate-700/60 pb-4">
                            <span class="text-slate-400 font-medium text-sm">Dia da Semana</span>
                            <span class="text-slate-400 font-medium text-sm">Horário</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Segunda-feira</span>
                            <span class="text-brand-300 bg-brand-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-brand-500/30">08:00 - 18:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Terça-feira</span>
                            <span class="text-brand-300 bg-brand-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-brand-500/30">08:00 - 18:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Quarta-feira</span>
                            <span class="text-brand-300 bg-brand-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-brand-500/30">08:00 - 18:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Quinta-feira</span>
                            <span class="text-brand-300 bg-brand-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-brand-500/30">08:00 - 18:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Sexta-feira</span>
                            <span class="text-brand-300 bg-brand-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-brand-500/30">08:00 - 18:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2 border-b border-slate-700/40">
                            <span class="font-semibold text-slate-200">Sábado</span>
                            <span class="text-emerald-300 bg-emerald-950/80 px-3 py-1 rounded-full text-xs font-semibold border border-emerald-500/30">08:00 - 12:00</span>
                        </div>

                        <div class="flex items-center justify-between py-2">
                            <span class="font-semibold text-slate-400">Domingo</span>
                            <span class="text-rose-400 bg-rose-950/50 px-3 py-1 rounded-full text-xs font-semibold border border-rose-500/30">Fechado</span>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- LOCALIZAÇÃO E CONTATO -->
    <section id="contato" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-6 space-y-6">
                    <span class="px-3.5 py-1.5 rounded-full bg-brand-100 text-brand-700 text-xs font-bold uppercase tracking-wider">Fale Conosco</span>
                    <h2 class="font-display font-extrabold text-3xl sm:text-4xl text-slate-900">
                        Entre em contato com o Pet Blue
                    </h2>
                    <p class="text-slate-600">
                        Estamos à disposição para tirar dúvidas, agendar visitas e receber o seu companheiro com muito carinho!
                    </p>

                    <div class="space-y-4 pt-2">
                        <div class="flex items-start gap-4 p-4 rounded-2xl bg-slate-50 border border-slate-100">
                            <div class="w-10 h-10 rounded-xl bg-brand-600 text-white flex items-center justify-center shrink-0">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-900">Endereço</h4>
                                <p class="text-sm text-slate-600">Rua São Paulo, 150, Centro<br>Extrema - MG, 37640-000, Brasil</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4 p-4 rounded-2xl bg-slate-50 border border-slate-100">
                            <div class="w-10 h-10 rounded-xl bg-emerald-500 text-white flex items-center justify-center shrink-0">
                                <i class="fa-brands fa-whatsapp text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-900">WhatsApp</h4>
                                <p class="text-sm text-slate-600">+55 35 99244-1849</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4 p-4 rounded-2xl bg-slate-50 border border-slate-100">
                            <div class="w-10 h-10 rounded-xl bg-slate-800 text-white flex items-center justify-center shrink-0">
                                <i class="fa-regular fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-900">E-mail</h4>
                                <p class="text-sm text-slate-600">petblue2026@gmail.com</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-6 bg-brand-50 p-8 rounded-3xl border border-brand-100 text-center space-y-6">
                    <div class="w-20 h-20 bg-emerald-500 text-white rounded-full flex items-center justify-center text-4xl mx-auto shadow-lg shadow-emerald-500/30">
                        <i class="fa-brands fa-whatsapp"></i>
                    </div>
                    
                    <h3 class="font-display font-bold text-2xl text-slate-900">Agende direto pelo WhatsApp</h3>
                    <p class="text-slate-600 text-sm max-w-md mx-auto">
                        Clique no botão abaixo para iniciar uma conversa instantânea com nossa equipe no WhatsApp!
                    </p>

                    <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20gostaria%20de%20agendar%20um%20servi%C3%A7o%20para%20meu%20pet." 
                       target="_blank"
                       class="inline-flex items-center justify-center gap-3 bg-emerald-500 hover:bg-emerald-600 text-white font-bold text-lg px-8 py-4 rounded-2xl shadow-lg transition-transform hover:scale-105">
                        <i class="fa-brands fa-whatsapp text-2xl"></i>
                        <span>Abrir Conversa no WhatsApp</span>
                    </a>
                </div>

            </div>
        </div>
    </section>

    <!-- BANNER WHATSAPP -->
    <section class="py-12 bg-gradient-to-r from-brand-700 to-brand-900 text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col sm:flex-row items-center justify-between gap-6">
            <div class="space-y-1 text-center sm:text-left">
                <h3 class="font-display font-extrabold text-2xl">Procurando cuidados com amor para seu Pet?</h3>
                <p class="text-brand-200 text-sm">Fale com a gente e saiba mais sobre o Pet Sitter, Hostel e Day Care.</p>
            </div>
            <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20gostaria%20de%20informa%C3%A7%C3%B5es." 
               target="_blank"
               class="bg-emerald-500 hover:bg-emerald-600 text-white font-bold px-8 py-4 rounded-2xl shadow-lg shrink-0 flex items-center gap-3 transition-all transform hover:scale-105">
                <i class="fa-brands fa-whatsapp text-2xl"></i>
                <span>Chamar no WhatsApp</span>
            </a>
        </div>
    </section>

    <!-- RODAPÉ -->
    <footer class="bg-navy-900 text-slate-400 py-12 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <div class="space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-xl bg-brand-600 flex items-center justify-center text-white font-bold">
                            <i class="fa-solid fa-paw"></i>
                        </div>
                        <span class="font-display font-extrabold text-xl text-white">Pet<span class="text-brand-500">Blue</span></span>
                    </div>
                    <p class="text-xs text-slate-400 leading-relaxed">
                        Desde 2021 oferecendo experiências únicas para o seu Pet com amor, dedicação e segurança em Extrema - MG.
                    </p>
                </div>

                <div>
                    <h4 class="text-white font-bold text-sm mb-4">Serviços</h4>
                    <ul class="space-y-2 text-xs">
                        <li><a href="#servicos" class="hover:text-brand-400 transition-colors">Pet Sitter</a></li>
                        <li><a href="#servicos" class="hover:text-brand-400 transition-colors">Pet Hostel</a></li>
                        <li><a href="#servicos" class="hover:text-brand-400 transition-colors">Day Care (Creche)</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-white font-bold text-sm mb-4">Navegação</h4>
                    <ul class="space-y-2 text-xs">
                        <li><a href="#sobre" class="hover:text-brand-400 transition-colors">Sobre Nós</a></li>
                        <li><a href="#horarios" class="hover:text-brand-400 transition-colors">Horários de Funcionamento</a></li>
                        <li><a href="#contato" class="hover:text-brand-400 transition-colors">Contato & Endereço</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-white font-bold text-sm mb-4">Redes Sociais</h4>
                    <div class="flex space-x-3">
                        <a href="https://instagram.com/petblue_extrema" target="_blank" class="w-9 h-9 rounded-xl bg-slate-800 hover:bg-brand-600 hover:text-white flex items-center justify-center text-slate-300 transition-colors">
                            <i class="fa-brands fa-instagram text-base"></i>
                        </a>
                        <a href="https://wa.me/5535992441849" target="_blank" class="w-9 h-9 rounded-xl bg-slate-800 hover:bg-emerald-500 hover:text-white flex items-center justify-center text-slate-300 transition-colors">
                            <i class="fa-brands fa-whatsapp text-base"></i>
                        </a>
                    </div>
                    <p class="text-[11px] text-slate-500 mt-4">Rua São Paulo, 150, Centro - Extrema/MG</p>
                </div>
            </div>

            <div class="border-t border-slate-800 pt-6 text-center text-xs text-slate-500">
                <p>&copy; 2026 Pet Blue Extrema. Todos os direitos reservados. "VOCÊ E SEU PET TRANQUILOS!"</p>
            </div>
        </div>
    </footer>

    <!-- BOTÃO FLUTUANTE WHATSAPP -->
    <a href="https://wa.me/5535992441849?text=Ol%C3%A1!%20Vim%20pelo%20site%20e%20gostaria%20de%20informa%C3%A7%C3%B5es." 
       target="_blank" 
       class="fixed bottom-6 right-6 z-50 bg-emerald-500 hover:bg-emerald-600 text-white w-14 h-14 rounded-full shadow-2xl flex items-center justify-center text-3xl transition-transform hover:scale-110">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

    <!-- JAVASCRIPT DO MENU MOBILE -->
    <script>
        const menuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>