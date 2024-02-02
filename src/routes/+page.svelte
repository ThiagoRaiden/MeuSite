<script lang="ts">
    import { Parallax, ParallaxLayer } from "svelte-parallax";
    import focaIlustation from "$lib/assets/ilustracoes/foca.png";
    import bolha from "$lib/assets/ilustracoes/bolha.png";
    import livro from "$lib/assets/ilustracoes/amazing.png";
    import sunsational from "$lib/assets/ilustracoes/sunsational.png";
    import gosma from "$lib/assets/ilustracoes/amoebaAmarela.png";
    import cardImg from "$lib/assets/banana.png";
    import rosto from "$lib/assets/ilustracoes/rosto.png";
    import * as Carousel from "$lib/components/ui/carousel/index.js";

    const shadow = "shadow-[0px_-20px_30px_15px_#F2C063]";
</script>

<Parallax sections={3} config={{ stiffness: 0.2, damping: 0.4 }}>
    <ParallaxLayer class="z-20 bg-background z-30 relative">
        <img
            class="absolute w-40 left-[50px] top-[50px] animate-wiggle"
            src={sunsational}
            alt=""
        />
        <img
            class="absolute w-48 right-[100px] top-[50px] animate-wiggle"
            src={focaIlustation}
            alt=""
        />
        <div
            class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12 h-full items-center relative"
        >
            <div class="mr-auto place-self-center lg:col-span-6">
                <h1
                    class=" mb-4 text-6xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    HI EVERYONE!
                </h1>
                <p class=" mb-6 font-Bryndan lg:mb-8 text-2xl lg:text-3xl">
                    <u>I'm Thiago Pastore Rubio</u>
                </p>
                <p
                    class=" mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl text-justify indent-20"
                >
                    Meu maior objetivo é inspirar meus alunos. A única maneira
                    de se tornar fluente em idioma é tornando ele parte do seu
                    dia-a-dia! Por isso meu maior esforço está em unir aquilo
                    que você já gosta de fazer todos os dias, com a prática do
                    inglês, pra que isso se torne um hábito diário!
                </p>

                <a
                    href="#"
                    class="inline-flex items-center justify-center px-5 py-3 text-base font-medium text-center text-gray-900 border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800"
                >
                    Speak to Sales
                </a>
            </div>
            <div class="hidden lg:mt-0 lg:col-span-6 lg:flex">
                <img src={rosto} alt="mockup" />
            </div>
        </div>
    </ParallaxLayer>
    <!--
       <ParallaxLayer class="bg-primary {shadow}" offset={0.99} rate={1.5}>
        <h1
            class="m-4 text-5xl font-extrabold tracking-tight leading-none font-Jingle text-center"
        >
            Depoimentos
        </h1>
    </ParallaxLayer> 
    -->

    <ParallaxLayer
        offset={1.3}
        rate={-0.5}
        style="display: flex; justify-content: flex-end;"
        class="z-20 "
    >
        <div
            style=" 
         height: 100%; "
            class="mx-15 w-1/2 z-0 bg-primary z-0 px-10 py-5 boderStyle"
        >
            <h1
                class="mb-4 text-6xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle text-red-300"
            >
                Aprenda do seu jeito!
            </h1>

            <div class="flex items-center justify-between">
                <h2
                    class="mb-4 text-6xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    No seu tempo!
                </h2>
                <div class="w-24 self-end">
                    <img src={livro} alt="mockup" class="   " />
                </div>
            </div>
            <p class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl">
                Você escolhe quando e quanto tempo de aula for melhor para você!
            </p>
            <h2
                class="mb-4 text-6xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
            >
                Do seu jeito!
            </h2>
            <p class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl">
                As aulas são personalizadas de acordo com as suas necessidades e
                a sua personalidade.
            </p>
            <h2
                class="mb-4 text-6xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
            >
                Flexibilidade!
            </h2>
            <p class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl">
                Precisou faltar? Não tem problema! Desde que avisado com
                antecedência, as aulas poderão ser repostas.
            </p>
        </div>
    </ParallaxLayer>

    <ParallaxLayer
        offset={1.1}
        rate={-0.1}
        style="display: flex; justify-content: flex-start; z-10"
    >
        <div
            style=" height: 100%; "
            class="mx-5 w-1/2 bg-secondary px-10 py-5 boderStyle2"
        >
            <h1
                class="mb-4 text-6xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle"
            >
                O que está incluso?
            </h1>

            <ol class=" list-inside before">
                <h2
                    class="mb-4 text-6xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Material
                </h2>

                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >1.</span
                        >
                    </div>
                    Livro completo em PDF.
                </li>

                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >2.</span
                        >
                    </div>
                    Livro de exercícios completo em PDF.
                </li>

                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >3.</span
                        >
                    </div>
                    Material Extra: Listas de exercícios e material online.
                </li>
            </ol>

            <h2
                class="mb-4 text-6xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
            >
                Suporte
            </h2>

            <ol class="list-inside">
                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >1.</span
                        >
                    </div>
                    Tire dúvidas quando precisar através do What’s App!
                </li>

                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >2.</span
                        >
                    </div>
                    Aulas gravadas!
                </li>

                <li
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl flex items-center gap-1"
                >
                    <div class="w-12 h-12 relative">
                        <img class="absolute z-0" src={gosma} alt="" />
                        <span
                            class="z-20 absolute w-full h-full flex items-center justify-center"
                            >3.</span
                        >
                    </div>
                    Clube de conversação uma vez ao mês!
                </li>
            </ol>
        </div>
    </ParallaxLayer>

    <ParallaxLayer offset={2.0} class="z-30 bg-accent">
        <Carousel.Root>
            <Carousel.Content>
                {#each { length: 10 } as _, i}
                    <Carousel.Item class="basis-1/5"
                        ><img src={cardImg} alt="" /></Carousel.Item
                    >
                {/each}
            </Carousel.Content>
        </Carousel.Root></ParallaxLayer
    >
</Parallax>

<style>
    .splash {
        width: 500px;
        height: 500px;
        background:
            repeating-conic-gradient(#00f 0 3%, #0000 0 11%),
            repeating-conic-gradient(#0000 0 5%, #00f 0 7%) 50% / 60% 60%,
            repeating-conic-gradient(#0000 0 7%, #00f 0 9%) 50% / 70% 70%,
            repeating-conic-gradient(#0000 0 11%, #00f 0 13%) 50% / 80% 80%,
            radial-gradient(#00f 22%, #0000 0),
            #fff;
        background-repeat: no-repeat;
        filter: blur(20px) contrast(50);
        box-shadow: 0 0 0 50px #fff;
    }

    .boderStyle {
        border-radius: 31% 69% 23% 77% / 66% 18% 82% 34%;
    }

    .boderStyle2 {
        border-radius: 22% 78% 57% 43% / 62% 49% 51% 38%;
    }

    li::before {
        background-image: url("lib/assets/ilustracoes/bolha.png");
    }

    li {
        background-size: 20px;
    }
</style>
