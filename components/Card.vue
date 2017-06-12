<template>
<div>
    <div class="thumbnail">
        <img :src=champ.thumbnail alt=" ">
        <div class="caption">
            <h5>{{champ.first_name}} {{champ.last_name}}</h5>
            <p class="weightclass">{{champ.weight_class}}</p>
            <div class="stats"> 
                <span class="body">Wins <span class="badge win"> {{ champ.wins }} </span></span> 
                <span class="body"> Draws <span class="badge"> {{ champ.draws }} </span></span>
                <span class="body"> Losses <span class="badge loss"> {{ champ.losses }} </span></span>
            </div>
        </div>
    </div>
</div>
</template>

<script>
    export default {
      props: ['champ']
    }
</script>

<style>
    .thumbnail{
        position: relative;
		background-color: #fff;
		max-width: 650px;
		padding: 30px 0px 10px;
		margin: 15px auto;
        border: 1px solid #e0e0e0;
		border-radius: 4px;
		box-shadow: 0 20px 20px rgba(0,0,0,.08);
		transition: all 250ms cubic-bezier(.02, .01, .47, 1);
    }
    .caption{
        text-align: center;
    }
    .weightclass{
        color: #af8686;
        font-weight: 500;
    }
    .stats .body{
        font-size: 12px;
        padding: 2px;
    }

</style>
