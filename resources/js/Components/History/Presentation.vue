<template>
    <div class="historyPresentation flex items-center flex-col">
        <h2 class="py-32 text-4xl">Le Sacré-Coeur : une église pour sauver la France</h2>
        <h3 class="w-3/4 mx-auto text-center">Nous sommes en 1870, en quelques semaines, l’histoire de la France va prendre un nouveau tournant. Le 19 juillet la France déclare la guerre à la Prusse mais dès le 2 septembre, Napoléon III est contraint de déposer les armes au terme de la bataille de Sedan et le 4 septembre la Troisième république est proclamée : c’est la fin du Second Empire. Pour autant, la guerre avec la Prusse n’est pas encore terminée et Paris est assiégée pendant plus de quatre mois. Le froid et la faim rendent ce siège particulièrement difficile pour les parisiens contraints de se nourrir de chevaux, de chats, de chiens, de rats et même des animaux du jardin des plantes (chameau, éléphant, antilope) que l’on est contraint de sacrifier ! En décembre 1870, Victor Hugo témoigne : “Ce n’est même plus du cheval que nous mangeons. C’est peut-être du chien ? C’est peut-être du rat ? Je commence à avoir des maux d’estomac. Nous mangeons de l’inconnu.”</h3>
        <div class="historyPart flex items-end p-32 gap-36 hideme">
            <img src="img/war.jpeg" class="h-96 mx-auto">
            <p>Le 18 janvier 1871, l’Empire Allemand est proclamé dans la galerie des glaces du château de Versailles et le 26 janvier un cessez-le-feu est signé. Pour autant, certains parisiens refusent de rendre. Le 18 mars, Adolphe Thiers envoie l’armée pour s’emparer des 227 canons installés sur la butte Montmartre. La manœuvre est mal préparée et échoue : les officiers sont désarmés par la foule. C’est alors le début de la Commune de Paris, une insurrection de plus de deux mois qui met la capitale à feu et à sang.</p>
        </div>
        <div class="historyPart flex items-end p-32 gap-36 hideme">
            <p>Cette période compliquée, commencée en 1789 avec la Révolution, est vue par certains catholiques comme une punition divine si bien que deux parisiens en exil, Hubert Rohault de Fleury et Alexandre Legentil, promettent de construire une nouvelle église si Dieu sauve la France.</p>
            <img src="img/hdv.jpeg" class="h-96 mx-auto">
        </div>
        <h2>La construction du Sacré-Cœur</h2>
        <div class="flex">
            <div class="historyPart p-32 hideme">
                <img src="img/construction1.jpeg" class="h-96 mx-auto pb-10">
                <p>Une fois la situation apaisée, on décide d’ériger ladite église sur la butte Montmartre, lieu symbolique du début de la Commune de Paris et où Saint Denis a été décapité. Le projet fait débat, certains y voient le symbole de l’église sur la Révolution, pourtant en 1873 une loi reconnaît l’église d’utilité publique et une vaste souscription nationale est lancée pour en financer la construction. Les Français sont appelés à participer à la hauteur de leurs moyens, un programme qui rencontre un vif succès grâce à la “souscription des pierres” qui incite la population à réunir des fonds pour l’achat d’une pierre, d’une colonne voire d’une chapelle sur lesquels on grave les initiales ou le nom des donateurs. Les travaux sont achevés mais la consécration prévue en octobre 1914 est reportée en raison de la guerre et n’aura lieu qu’en 1919.</p>
            </div>
            <div class="historyPart p-32 hideme">
                <img src="img/construction2.jpeg" class="h-96 mx-auto pb-10">
                <p>Bien que parfois décrié par certains qui voient dans son architecture un “gâteau surmonté de Chantilly”, le Sacré-Cœur est aujourd’hui bien installé dans le paysage parisien et fait le bonheur des montmartrois autant que des touristes : après Notre-Dame c’est le deuxième monument parisien le plus visité.</p>
            </div>
        </div>
        <h2>Visite du dôme du Sacré-Cœur</h2>
        <div class="historyPart p-32 hideme">
            <img src="img/dome-sacre-coeur-3.jpeg" class="h-96 mx-auto pb-10">
            <p>Que l’on apprécie ou non l’architecture du Sacré-Cœur, la vue que l’on a sur Paris depuis son parvis est à couper le souffle ! Et pour en profiter encore davantage, rien de mieux que de prendre encore plus de hauteur en montant sur le dôme de l’église.</p>
        </div>
        <div class="historyPart flex items-end p-32 gap-36 hideme">
            <img src="img/dome-sacre-coeur-4.jpeg" class="h-96 mx-auto">
            <p class="w-2/4">Quelques 300 marches sont à gravir pour atteindre les parties hautes du Sacré-Cœur mais la récompense est à la hauteur de l’effort : une vue à 360° sur le centre et le nord de Paris. Vous pourrez de plus observer les gargouilles de très près !</p>
        </div>
        <div class="historyPart flex items-end p-32 gap-36 hideme">
            <p class="w-2/4">Si l’entrée du Sacré-Cœur est gratuite, l’accès au dôme est quant à lui payant : 7€ par personne.</p>
            <img src="img/dome-sacre-coeur-5.jpeg" class="h-96 mx-auto">
        </div>
        <div class="flex pb-32">
            <div class="historyPart hideme">
                <img src="img/dome-sacre-coeur.jpeg" class="h-96 mx-auto pb-10">
                <p class="w-3/4 mx-auto">Pol.Est gratis clabulaA falsis, cThe souHow cold. You loot like a mast.rce shapes.lassis azureus frondator.re, cesaris.</p>
            </div>
            <div class="historyPart hideme">
                <img src="img/dome-sacre-coeur-2.jpeg" class="h-96 mx-auto pb-10">
                <p class="w-3/4 mx-auto">Pol.Est gratis clabulaA falsis, cThe souHow cold. You loot like a mast.rce shapes.lassis azureus frondator.re, cesaris.</p>
            </div>
        </div>

    </div>
</template>
<script>
    export default {
        name : 'historyPresentation'
    }

$(document).ready(function() {


    $(window).scroll( function(){

        $('.hideme').each( function(i){

            var bottom_of_object = $(this).offset().top + 500;
            var bottom_of_window = $(window).scrollTop() + $(window).height();

            if( bottom_of_window > bottom_of_object ){

                $(this).animate({'opacity':'1'},1000);

            }

        }); 

    });

});

</script>

<style>

    .historyPresentation {
        background-image: url('/img/lyonnette.png');
        background-attachment: fixed;
    }

    .historyPresentation p {
        font-weight: 500;
        font-size: 20px;
        text-align: justify;
    }

    .historyPresentation h2 {
        font-size: 30px;
        font-weight: 600;
    }

    .historyPresentation h3 {
        font-weight: 400;
    }

    .historyPresentation img {
        border-radius: 30px;
    }

    .hideme {
        opacity: 0;
    }

</style>
