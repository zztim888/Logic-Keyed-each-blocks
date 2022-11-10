<script>
    const countries = {
        Sweden: 'sthlm',
        Norway: 'Oslo',
        Denmark: 'Copenhagen'
    }
    export let countryName;

    const country = countries[countryName];
    
</script>

<p>
    <span>The country {countryName} has the capital {country}</span>
</p>

<style>
    p{
        margin:0.5em;
    }
    span{
        display: inline-block;
        background-color: lightskyblue;
        color: white;
        padding: 0.2em 0.3em 0.2em;
        border-radius: 0.7em;
        text-align: center;
    }
    span:hover{
        background-color: rgb(187, 112, 127);        
    }
</style>