<script lang="ts">
    import { Parallax, ParallaxLayer } from "svelte-parallax";
    import livro from "$lib/assets/ilustracoes/amazing.png";
    import gosma from "$lib/assets/ilustracoes/amoebaAmarela.png";
    import cardImg from "$lib/assets/banana.png";
    import danilo from "$lib/assets/danilo.png";
    import ana from "$lib/assets/Ana.png";
    import aline from "$lib/assets/Aline.png";   
    import daniel from "$lib/assets/daniel.png";
    import felipe from "$lib/assets/Felipe.png";
    import gabrielzinho from "$lib/assets/gabrielzinho.png";
    import guilherme from "$lib/assets/guilherme.png";
    import heloisa from "$lib/assets/heloisa.png";
    import priscila from "$lib/assets/Priscila.png";
    import rafael from "$lib/assets/Rafael.png";
    import sabryna from "$lib/assets/Sabryna.png";
    import suzan from "$lib/assets/suzan.png";
    import vihn from "$lib/assets/Vihn.png";
    import weil from "$lib/assets/weil.png";
    import tiemi from "$lib/assets/Tiemi.png";
    import lia from "$lib/assets/Lia.png";
    import leonildo from "$lib/assets/leonildo.png";
    import antonio from "$lib/assets/Antonio.png";
    import kevin from "$lib/assets/kevin.png";
    import gabriel from "$lib/assets/gabriel.png";

    import * as Carousel from "$lib/components/ui/carousel/index.js";
    import HeroContentIntro from "./HeroContentIntro.svelte";

    const shadow = "shadow-[0px_-20px_30px_15px_#F2C063]";
    let innerWidth: number;
    $: console.log(innerWidth);

    const suportItems = [
        "Tire dúvidas quando precisar através do What’s App!",
        "Aulas gravadas!",
        " Clube de conversação uma vez ao mês!",
    ];
    const materialItems = [
        "Livro completo em PDF.",
        "Livro de exercícios completo em PDF.",
        "Material Extra: Listas de exercícios e material online.",
    ];
</script>

<svelte:window bind:innerWidth />

<Parallax sections={4} config={{ stiffness: 0.2, damping: 0.4 }}>
    <ParallaxLayer class="bg-background z-30 relative">
        <HeroContentIntro />
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
    {#if innerWidth > 1200}
        <ParallaxLayer
            offset={1.3}
            rate={-0.5}
            style="display: flex; justify-content: flex-end;"
            class="z-20 "
        >
            <div
                style=" 
         height: 100%; "
                class="mx-15 w-1/2 bg-primary z-0 px-10 py-5 boderStyle"
            >
                <h1
                    class="mb-4 text-6xl md:text-8xl lg:text-6xl font-extrabold tracking-tight leading-none font-Jingle text-red-300"
                    style="  text-shadow:
                    3px 3px 2px #000,
                    -3px 3px 2px #000,
                    -3px -3px 0 #000,
                    3px -3px 0 #000;"
                >
                    Aprenda do seu jeito!
                </h1>

                <div class="flex items-center justify-between">
                    <h2
                        class="mb-4 text-6xl md:text-8xl lg:text-4xl font-extrabold tracking-tight leading-none font-Jingle"
                    >
                        No seu tempo!
                    </h2>
                    <div class="w-24 self-end">
                        <img src={livro} alt="mockup" class="   " />
                    </div>
                </div>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-2xl text-xl"
                >
                    Você escolhe quando e quanto tempo de aula for melhor para
                    você!
                </p>
                <h2
                    class="mb-4 text-6xl md:text-6xl lg:text-4xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Do seu jeito!
                </h2>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-2xl text-xl"
                >
                    As aulas são personalizadas de acordo com as suas
                    necessidades e a sua personalidade.
                </p>
                <h2
                    class="mb-4 text-6xl md:text-6xl lg:text-4xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Flexibilidade!
                </h2>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-2xl text-xl"
                >
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
                    class="mb-4 text-6xl md:text-8xl lg:text-4xl font-extrabold tracking-tight leading-none font-Jingle text-primary"
                    style="  text-shadow:
                    3px 3px 2px #000,
                    -3px 3px 2px #000,
                    -3px -3px 0 #000,
                    3px -3px 0 #000;"
                >
                    O que está incluso?
                </h1>

                <ol class=" list-inside before">
                    <h2
                        class="mb-4 text-6xl md:text-8xl lg:text-3xl font-extrabold tracking-tight leading-none font-Jingle"
                    >
                        Material
                    </h2>

                    <li
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
                    class="mb-4 text-6xl md:text-8xl lg:text-3xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Suporte
                </h2>

                <ol class="list-inside">
                    <li
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
                        class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-xl text-xl flex items-center gap-1"
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
    {:else}
        <ParallaxLayer
            offset={1}
            style="display: flex; justify-content: flex-end;"
            class="z-20 "
        >
            <div
                style=" 
     height: 100%; "
                class="mx-15 w-full bg-primary z-0 px-10 py-5 boderStyle"
            >
                <h1
                    class="mb-4 text-4xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle text-red-300"
                    style="  text-shadow:
                    3px 3px 2px #000,
                    -3px 3px 2px #000,
                    -3px -3px 0 #000,
                    3px -3px 0 #000;"
                >
                    Aprenda do seu jeito!
                </h1>

                <div class="flex items-center justify-between">
                    <h2
                        class="mb-4 text-4xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                    >
                        No seu tempo!
                    </h2>
                    <div class="w-20 md:w-48 self-end">
                        <img src={livro} alt="mockup" class="   " />
                    </div>
                </div>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl"
                >
                    Você escolhe quando e quanto tempo de aula for melhor para
                    você!
                </p>
                <h2
                    class="mb-4 text-4xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Do seu jeito!
                </h2>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl"
                >
                    As aulas são personalizadas de acordo com as suas
                    necessidades e a sua personalidade.
                </p>
                <h2
                    class="mb-4 text-4xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Flexibilidade!
                </h2>
                <p
                    class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl"
                >
                    Precisou faltar? Não tem problema! Desde que avisado com
                    antecedência, as aulas poderão ser repostas.
                </p>
            </div>
        </ParallaxLayer>
        <ParallaxLayer
            offset={2}
            style="display: flex; justify-content: flex-start; z-10"
        >
            <div
                style=" height: 100%; "
                class="mx-5 w-full bg-secondary px-10 py-5 boderStyle2"
            >
                <h1
                    class="mb-4 text-4xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle text-primary"
                    style="  text-shadow:
                    3px 3px 2px #000,
                    -3px 3px 2px #000,
                    -3px -3px 0 #000,
                    3px -3px 0 #000;"
                >
                    O que está incluso?
                </h1>

                <ol class="list-inside">
                    {#each materialItems as item, idx}
                        <li
                            class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl grid grid-cols-12 items-center"
                        >
                            <div class="w-12 h-12 relative col-span-2">
                                <img class="absolute z-0" src={gosma} alt="" />
                                <span
                                    class="z-20 absolute w-full h-full flex items-center justify-center"
                                    >{idx + 1}.</span
                                >
                            </div>
                            <p class="col-span-10 pl-2">{item}</p>
                        </li>
                    {/each}
                </ol>

                <h2
                    class="mb-4 text-4xl md:text-8xl lg:text-5xl font-extrabold tracking-tight leading-none font-Jingle"
                >
                    Suporte
                </h2>
                <ol class="list-inside">
                    {#each suportItems as item, idx}
                        <li
                            class="mb-6 font-Bryndan lg:mb-8 md:text-lg lg:text-3xl text-xl grid grid-cols-12 items-center"
                        >
                            <div class="w-12 h-12 relative col-span-2">
                                <img class="absolute z-0" src={gosma} alt="" />
                                <span
                                    class="z-20 absolute w-full h-full flex items-center justify-center"
                                    >{idx + 1}.</span
                                >
                            </div>
                            <p class="col-span-10 pl-2">{item}</p>
                        </li>
                    {/each}
                </ol>
            </div>
        </ParallaxLayer>
    {/if}

    <ParallaxLayer offset={3} class="z-30 bg-accent grid items-center">
        <div class="">
            <h1
                class="mb-4 text-5xl md:text-8xl lg:text-8xl font-extrabold tracking-tight leading-none font-Jingle text-center"
            >
                Depoimentos
            </h1>
            <Carousel.Root>
                <Carousel.Content>
                    <Carousel.Item
                            class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                            >
                            <img src={danilo} alt="" />
                            
                            </Carousel.Item
                        >
                    
                        <Carousel.Item
                            class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                            >
                            <img src={kevin} alt="" />
                            
                            </Carousel.Item
                        >
                        <Carousel.Item
                        class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                        >
                        <img src={ana} alt="" />
                        
                        </Carousel.Item
                    >
                    <Carousel.Item
                    class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                    >
                    <img src={antonio} alt="" />
                    
                    </Carousel.Item
                >
                <Carousel.Item
                class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                >
                <img src={daniel} alt="" />
                
                </Carousel.Item
            >
            <Carousel.Item
            class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
            >
            <img src={felipe} alt="" />
            
            </Carousel.Item
        >
        <Carousel.Item
        class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
        >
        <img src={sabryna} alt="" />
        
        </Carousel.Item
    >
    <Carousel.Item
    class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
    >
    <img src={gabrielzinho} alt="" />
    
    </Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={guilherme} alt="" />

</Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={heloisa} alt="" />

</Carousel.Item
>

<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={leonildo} alt="" />

</Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={lia} alt="" />

</Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={priscila} alt="" />

</Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={rafael} alt="" />

</Carousel.Item
>    
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={vihn} alt="" />

</Carousel.Item
>   
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={weil} alt="" />

</Carousel.Item
>       

<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={tiemi} alt="" />

</Carousel.Item
>
<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={aline} alt="" />

</Carousel.Item
>

<Carousel.Item
class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
>
<img src={gabriel} alt="" />

</Carousel.Item
>

<Carousel.Item
                            class={innerWidth > 900 ? "basis-1/2" : "basis-1/2"}
                            >
                            <img src={suzan} alt="" />
                            
                            </Carousel.Item
                        >
 
                        
                 
                </Carousel.Content>
            </Carousel.Root>
        </div>
    </ParallaxLayer>
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

    li {
        background-size: 20px;
    }
</style>
