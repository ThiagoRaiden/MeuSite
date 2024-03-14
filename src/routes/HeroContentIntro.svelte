<script>
    import focaIlustation from "$lib/assets/ilustracoes/foca.png";
    import rosto from "$lib/assets/ilustracoes/rosto.png";
    import wppLogo from "$lib/assets/ilustracoes/wpp.png"
    import sunsational from "$lib/assets/ilustracoes/sunsational.png";
</script>

<img
    class="absolute w-20 md:w-40 lg:w-40 sm:left-[10px] animate-wiggle"
    src={sunsational}
    alt=""
/>
<img
    class="absolute w-20 md:w-48 lg:w-48 sm:bottom-[50px] md:top-[50px] right-[50px] animate-wiggle"
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
            class="mb-6 font-Bryndan md:text-lg lg:text-3xl text-xl text-justify indent-20"
        >
            Meu maior objetivo é inspirar meus alunos. A única maneira de se
            tornar fluente em idioma é tornando ele parte do seu dia-a-dia! Por
            isso meu maior esforço está em unir aquilo que você já gosta de
            fazer todos os dias, com a prática do inglês, pra que isso se torne
            um hábito diário!
        </p>
        <div
            class="mb-6 mt-2 font-Bryndan md:text-lg lg:text-3xl text-xl text-center"
        >
        <div class="flex gap-2 justify-center">
            <img src={wppLogo} alt="mockup" class="h-10 w-10" />(41) 99781-9786 
        </div>
        
         
            ou <br><a
                href="agenda"
                class="inline-flex items-center justify-center px-5 py-3 text-base font-medium text-center text-gray-900 border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800"
            >
                Agende uma aula experimental
            </a>
        </div>
    </div>
    <div class="hidden lg:mt-0 lg:col-span-6 lg:flex">
        <img src={rosto} alt="mockup" />
    </div>
</div>
