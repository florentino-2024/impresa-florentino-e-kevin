<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Florentino & Kevin | Tecnologia e Software</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8fafc;
        }
        
        .gradient-bg {
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 100%);
        }
        
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #3b82f6;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover:after {
            width: 100%;
        }
        
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
            100% { transform: translateY(0px); }
        }
    </style>
</head>
<body>
    <!-- Header/Navigation -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <!-- Logo -->
                <div class="flex items-center">
                    <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center text-white font-bold text-xl mr-3">
                        FK
                    </div>
                    <h1 class="text-xl font-bold text-gray-800">Florentino & Kevin</h1>
                </div>
                
                <!-- Mobile menu button -->
                <div class="md:hidden">
                    <button id="menu-toggle" class="text-gray-500 hover:text-gray-700 focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
                
                <!-- Desktop Navigation -->
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link text-gray-600 hover:text-gray-900 font-medium">Início</a>
                    <a href="#services" class="nav-link text-gray-600 hover:text-gray-900 font-medium">Serviços</a>
                    <a href="#about" class="nav-link text-gray-600 hover:text-gray-900 font-medium">Sobre Nós</a>
                    <a href="#portfolio" class="nav-link text-gray-600 hover:text-gray-900 font-medium">Portfólio</a>
                    <a href="#contact" class="nav-link text-gray-600 hover:text-gray-900 font-medium">Contato</a>
                </nav>
            </div>
            
            <!-- Mobile Navigation -->
            <div id="mobile-menu" class="hidden md:hidden mt-4 pb-4">
                <a href="#home" class="block py-2 text-gray-600 hover:text-gray-900">Início</a>
                <a href="#services" class="block py-2 text-gray-600 hover:text-gray-900">Serviços</a>
                <a href="#about" class="block py-2 text-gray-600 hover:text-gray-900">Sobre Nós</a>
                <a href="#portfolio" class="block py-2 text-gray-600 hover:text-gray-900">Portfólio</a>
                <a href="#contact" class="block py-2 text-gray-600 hover:text-gray-900">Contato</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white py-20">
        <div class="container mx-auto px-6 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold leading-tight mb-6">Soluções Tecnológicas para o Futuro</h1>
                <p class="text-xl mb-8">Na Florentino & Kevin, transformamos ideias em realidade digital com soluções personalizadas e inovadoras.</p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#contact" class="bg-white text-blue-600 hover:bg-gray-100 px-8 py-3 rounded-lg font-semibold text-center transition duration-300">Fale Conosco</a>
                    <a href="#services" class="border-2 border-white text-white hover:bg-white hover:text-blue-600 px-8 py-3 rounded-lg font-semibold text-center transition duration-300">Nossos Serviços</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="https://cdn-icons-png.flaticon.com/512/3271/3271488.png" alt="Hero Image" class="w-3/4 md:w-full max-w-md animate-float">
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">Nossos Serviços</h2>
                <div class="w-20 h-1 bg-blue-500 mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Oferecemos soluções completas em tecnologia e software para impulsionar o seu negócio.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-code text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Desenvolvimento de Software</h3>
                        <p class="text-gray-600">Soluções personalizadas de software para atender às necessidades específicas do seu negócio.</p>
                    </div>
                </div>
                
                <!-- Service 2 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-mobile-alt text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Aplicativos Móveis</h3>
                        <p class="text-gray-600">Desenvolvimento de aplicativos iOS e Android com design intuitivo e alta performance.</p>
                    </div>
                </div>
                
                <!-- Service 3 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-globe text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Desenvolvimento Web</h3>
                        <p class="text-gray-600">Criação de websites responsivos e sistemas web com as melhores tecnologias do mercado.</p>
                    </div>
                </div>
                
                <!-- Service 4 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-cloud text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Soluções em Nuvem</h3>
                        <p class="text-gray-600">Migração, implementação e gerenciamento de infraestrutura em nuvem para sua empresa.</p>
                    </div>
                </div>
                
                <!-- Service 5 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-chart-line text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Business Intelligence</h3>
                        <p class="text-gray-600">Análise de dados e relatórios inteligentes para auxiliar na tomada de decisões estratégicas.</p>
                    </div>
                </div>
                
                <!-- Service 6 -->
                <div class="bg-white rounded-xl shadow-md overflow-hidden card-hover transition duration-300">
                    <div class="p-8">
                        <div class="gradient-bg w-16 h-16 rounded-full flex items-center justify-center text-white mb-6">
                            <i class="fas fa-shield-alt text-2xl"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-800 mb-3">Segurança da Informação</h3>
                        <p class="text-gray-600">Proteção de dados e sistemas com as melhores práticas e tecnologias de segurança digital.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <img src="https://cdn-icons-png.flaticon.com/512/3242/3242257.png" alt="About Us" class="w-full max-w-md mx-auto">
                </div>
                <div class="md:w-1/2">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-6">Sobre a Florentino & Kevin</h2>
                    <div class="w-20 h-1 bg-blue-500 mb-6"></div>
                    <p class="text-gray-600 mb-6">Fundada em 2023, a Florentino & Kevin nasceu da paixão por tecnologia e da vontade de criar soluções inovadoras que realmente fazem a diferença no mercado.</p>
                    <p class="text-gray-600 mb-6">Nossa equipe é composta por especialistas altamente qualificados em diversas áreas da tecnologia, unindo experiência técnica com criatividade para entregar os melhores resultados.</p>
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="gradient-bg w-8 h-8 rounded-full flex items-center justify-center text-white mr-4 mt-1">
                                <i class="fas fa-check text-sm"></i>
                            </div>
                            <p class="text-gray-600 flex-1">Comprometimento com a excelência em cada projeto</p>
                        </div>
                        <div class="flex items-start">
                            <div class="gradient-bg w-8 h-8 rounded-full flex items-center justify-center text-white mr-4 mt-1">
                                <i class="fas fa-check text-sm"></i>
                            </div>
                            <p class="text-gray-600 flex-1">Foco na inovação e nas últimas tendências tecnológicas</p>
                        </div>
                        <div class="flex items-start">
                            <div class="gradient-bg w-8 h-8 rounded-full flex items-center justify-center text-white mr-4 mt-1">
                                <i class="fas fa-check text-sm"></i>
                            </div>
                            <p class="text-gray-600 flex-1">Atendimento personalizado e suporte contínuo</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">Nosso Portfólio</h2>
                <div class="w-20 h-1 bg-blue-500 mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Alguns dos projetos que desenvolvemos com paixão e dedicação.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="rounded-xl overflow-hidden shadow-md card-hover transition duration-300">
                    <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Project 1" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Sistema de Gestão Empresarial</h3>
                        <p class="text-gray-600 mb-4">Plataforma completa para gestão de negócios com módulos integrados.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Web</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Cloud</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">BI</span>
                        </div>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="rounded-xl overflow-hidden shadow-md card-hover transition duration-300">
                    <img src="https://images.unsplash.com/photo-1555774698-0b77e0d5fac6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="Project 2" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Aplicativo de Delivery</h3>
                        <p class="text-gray-600 mb-4">Solução móvel para restaurantes com rastreamento em tempo real.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">iOS</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Android</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Backend</span>
                        </div>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="rounded-xl overflow-hidden shadow-md card-hover transition duration-300">
                    <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1415&q=80" alt="Project 3" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Plataforma de Analytics</h3>
                        <p class="text-gray-600 mb-4">Ferramenta de análise de dados com dashboards personalizáveis.</p>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Web</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Data Science</span>
                            <span class="bg-blue-100 text-blue-800 text-xs px-3 py-1 rounded-full">Visualização</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-12">
                <a href="#" class="inline-block gradient-bg text-white hover:bg-blue-600 px-8 py-3 rounded-lg font-semibold transition duration-300">Ver Mais Projetos</a>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">O Que Nossos Clientes Dizem</h2>
                <div class="w-20 h-1 bg-blue-500 mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">A satisfação dos nossos clientes é nossa maior recompensa.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 text-xl mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"A Florentino & Kevin revolucionou nosso sistema de gestão. O atendimento foi excelente e o produto final superou nossas expectativas."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/43.jpg" alt="Client 1" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-gray-800">Ana Silva</h4>
                            <p class="text-gray-600 text-sm">CEO, Empresa X</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-white p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 text-xl mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"O aplicativo desenvolvido pela equipe da Florentino & Kevin teve um impacto direto no aumento das nossas vendas. Profissionais altamente competentes."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Client 2" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-gray-800">Carlos Mendes</h4>
                            <p class="text-gray-600 text-sm">Diretor, Empresa Y</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-white p-8 rounded-xl shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 text-xl mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"Migramos toda nossa infraestrutura para nuvem com a Florentino & Kevin e os resultados foram impressionantes em termos de performance e redução de custos."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Client 3" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-gray-800">Juliana Oliveira</h4>
                            <p class="text-gray-600 text-sm">CTO, Empresa Z</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">Entre em Contato</h2>
                <div class="w-20 h-1 bg-blue-500 mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Tem um projeto em mente ou precisa de mais informações? Estamos aqui para ajudar.</p>
            </div>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h3 class="text-2xl font-bold text-gray-800 mb-6">Informações de Contato</h3>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white mr-4">
                                <i class="fas fa-map-marker-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Endereço</h4>
                                <p class="text-gray-600">Av. Paulista, 1000 - São Paulo, SP</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white mr-4">
                                <i class="fas fa-phone-alt"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Telefone</h4>
                                <p class="text-gray-600">(11) 1234-5678</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white mr-4">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800">Email</h4>
                                <p class="text-gray-600">contato@florentinoekevin.com.br</p>
                            </div>
                        </div>
                    </div>
                    
                    <h3 class="text-2xl font-bold text-gray-800 mt-10 mb-6">Nossas Redes Sociais</h3>
                    <div class="flex space-x-4">
                        <a href="#" class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white hover:bg-blue-600 transition duration-300">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white hover:bg-blue-600 transition duration-300">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white hover:bg-blue-600 transition duration-300">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="gradient-bg w-10 h-10 rounded-full flex items-center justify-center text-white hover:bg-blue-600 transition duration-300">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <form class="bg-white rounded-lg shadow-md p-8">
                        <div class="mb-6">
                            <label for="name" class="block text-gray-700 font-medium mb-2">Nome Completo</label>
                            <input type="text" id="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Seu nome">
                        </div>
                        
                        <div class="mb-6">
                            <label for="email" class="block text-gray-700 font-medium mb-2">Email</label>
                            <input type="email" id="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="seu@email.com">
                        </div>
                        
                        <div class="mb-6">
                            <label for="subject" class="block text-gray-700 font-medium mb-2">Assunto</label>
                            <input type="text" id="subject" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Qual o assunto?">
                        </div>
                        
                        <div class="mb-6">
                            <label for="message" class="block text-gray-700 font-medium mb-2">Mensagem</label>
                            <textarea id="message" rows="5" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent" placeholder="Sua mensagem..."></textarea>
                        </div>
                        
                        <button type="submit" class="w-full gradient-bg text-white hover:bg-blue-600 px-6 py-3 rounded-lg font-semibold transition duration-300">Enviar Mensagem</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="py-16 gradient-bg text-white">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-2xl md:text-3xl font-bold mb-6">Assine Nossa Newsletter</h2>
            <p class="max-w-2xl mx-auto mb-8">Mantenha-se atualizado com as últimas novidades, tendências tecnológicas e ofertas especiais da Florentino & Kevin.</p>
            
            <form class="max-w-md mx-auto flex">
                <input type="email" placeholder="Seu melhor email" class="flex-1 px-4 py-3 rounded-l-lg focus:outline-none text-gray-800">
                <button type="submit" class="bg-blue-800 hover:bg-blue-900 px-6 py-3 rounded-r-lg font-semibold transition duration-300">Assinar</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-4">
                        <div class="w-10 h-10 rounded-full gradient-bg flex items-center justify-center text-white font-bold text-xl mr-3">
                            FK
                        </div>
                        <h3 class="text-xl font-bold">Florentino & Kevin</h3>
                    </div>
                    <p class="text-gray-400">Transformando ideias em soluções tecnológicas inovadoras desde 2023.</p>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Links Rápidos</h4>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition duration-300">Início</a></li>
                        <li><a href="#services" class="text-gray-400 hover:text-white transition duration-300">Serviços</a></li>
                        <li><a href="#about" class="text-gray-400 hover:text-white transition duration-300">Sobre Nós</a></li>
                        <li><a href="#portfolio" class="text-gray-400 hover:text-white transition duration-300">Portfólio</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-white transition duration-300">Contato</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Serviços</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Desenvolvimento de Software</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Aplicativos Móveis</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Soluções Web</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Consultoria em TI</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Segurança da Informação</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-semibold mb-4">Contato</h4>
                    <ul class="space-y-2">
                        <li class="flex items-start">
                            <i class="fas fa-map-marker-alt text-gray-400 mr-2 mt-1"></i>
                            <span class="text-gray-400">Av. Paulista, 1000 - São Paulo, SP</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-phone-alt text-gray-400 mr-2 mt-1"></i>
                            <span class="text-gray-400">(11) 1234-5678</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-envelope text-gray-400 mr-2 mt-1"></i>
                            <span class="text-gray-400">contato@florentinoekevin.com.br</span>
                        </li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 Florentino & Kevin. Todos os direitos reservados.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-facebook-f"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-linkedin-in"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                        <i class="fab fa-instagram"></i>
                    </a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('menu-toggle').addEventListener('click', function() {
            document.getElementById('mobile-menu').classList.toggle('hidden');
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                
                // Close mobile menu if open
                document.getElementById('mobile-menu').classList.add('hidden');
            });
        });

        // Form submission (example)
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Obrigado por entrar em contato! Responderemos em breve.');
            this.reset();
        });
    </script>
</body>
</html>
