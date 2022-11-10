<script>
    const players = {
        Ronaldo: 'foward',
        RobertoCarlos: 'midfilder',
        Dida: 'goalkeeper'
    }

    export let playerPosition;

    const player = players[playerPosition]
</script>

<p>
    <span>The player {playerPosition} has the position {player}</span>
</p>

<style>
    p{
        margin:0.5em;
    }
    span{
        display: inline-block;
        background-color: lightblue;
        color: white;
        padding: 0.2em 0.3em 0.2em;
        border-radius: 0.7em;
        text-align: center;
    }
    span:hover{
        background-color: rgb(187, 112, 127);        
    }
</style>