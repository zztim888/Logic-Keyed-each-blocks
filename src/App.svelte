<script>
import Country from './Country.svelte';
import Player from './Player.svelte';
import Thing from './Thing.svelte';

let things = [
  {id: 1, name: 'apple'},
  {id: 2, name: 'banana'},
  {id: 3, name: 'carrot'},
  {id: 4, name: 'dougnut'},
  {id: 5, name: 'egg'} 
];

let countries = [
  {id:6, countryName: 'Sweden'},
  {id:7, countryName: 'Norway'},
  {id:8, countryName: 'Denmark'}
]

let players = [
  {id:9, playerPosition: 'Ronaldo'},
  {id:10, playerPosition: 'RobertoCarlos'},
  {id:11, playerPosition: 'Dida'}
]

function handleClick(){
  things = things.slice(1);
}

function countryClick(){
  countries = countries.slice(1);
}

function playerClick(){
  players = players.slice(1);
}
</script>

<button on:click={handleClick}>
 Remove first thing
</button>
<!-- you can write it in two diffrent ways -->
{#each things as thing(thing.id)}
<!-- this is a shortut -->
 <!-- {#each things as thing} -->
<Thing name={thing.name}/>
{/each}

<!----remove countries and capitals------>
<hr>
<button on:click={countryClick}>
  Remove first country
 </button>
 
 <!-- {#each countries as country (country.id)} -->
 {#each countries as country}
 <Country countryName={country.countryName}/>
 {/each}

 <!----remove players and their positions------>
<hr>
<button on:click={playerClick}>
  delete the first player
 </button>
 <!-- you write the code below in two different ways--> 
 <!--   {#each players as player(player.id)} -->
 {#each players as player(player.id)}
 <Player playerPosition={player.playerPosition}/>
 {/each}

 
 