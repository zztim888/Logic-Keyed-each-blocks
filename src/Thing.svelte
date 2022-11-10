<script>

    const emojis = {
        apple: "🍎",
        banana: "🍌",
        carrot: "🥕",
        dougnut: "🍩",
        egg: "🥚"
    }

    export let name;

    const emoji = emojis[name];
</script>

<p>
    <span> The emoji for the {name} is: {emoji}</span>
</p>

<style>
    p{
        margin:0.5em;
    }
    span{
        display: inline-block;
        background-color: pink;
        color: white;
        padding: 0.2em 0.3em 0.2em;
        border-radius: 0.7em;
        text-align: center;
    }
    span:hover{
        background-color: rgb(187, 112, 127);        
    }
</style>