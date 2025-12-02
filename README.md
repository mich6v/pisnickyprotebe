# pisnickyprotebe
images for www.pisnickyprotebe.cz

<div class="smart-image" style="--w: 100%; --h: 300px; --mobile-h: 250px;">
    
    <img 
        src="https://cdn.jsdelivr.net/gh/TVUJ_UZIVATEL/REPOZITAR/main/fotka.jpg" 
        alt="Popis" 
        loading="lazy"
    >
    
</div>

<style>
/* 1. Základní nastavení kontejneru */
.smart-image {
    /* Načte si hodnoty, které jsi zadal nahoře v HTML */
    width: var(--w);
    height: var(--h);
    
    /* Vzhled */
    border-radius: 16px;
    overflow: hidden;
    position: relative;
    background-color: #e0e0e0;
    
    /* Zarovnání (kdyby byla šířka menší než 100%, ať je to uprostřed) */
    margin: 0 auto; 
    max-width: 100%; /* Aby to nepřeteklo z obrazovky */
}

/* 2. Nastavení obrázku uvnitř */
.smart-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;   /* Ořízne fotku, aby seděla a nedeformovala se */
    object-position: center;
    display: block;
    
    /* Animace náběhu */
    animation: fadeIn 0.5s ease-in-out;
}

@keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

/* 3. MOBILNÍ VERZE (do 768px) */
@media (max-width: 768px) {
    .smart-image {
        /* Na mobilu vždy roztáhnout na plnou šířku */
        width: 100% !important;
        
        /* Výška na mobilu (načte si hodnotu --mobile-h nebo použije default 250px) */
        height: var(--mobile-h, 250px) !important;
    }
}
</style>
