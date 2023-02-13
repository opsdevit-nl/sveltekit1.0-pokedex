<script>
     /** @type {import('./$types').PageData} */
    export let data;
    const type = data.props.pokeman.types[0].type.name
</script>
<div class="flex flex-col items-center">
<h1 class="text-4xl text-center my-8 uppercase">{data.props.pokeman.name}</h1>
<p>Type: <strong>{type}</strong> | Height: <strong>{data.props.pokeman.height}</strong> | Weight: <strong>{data.props.pokeman.weight}</strong>
</p>
<img class="card-image" src={data.props.pokeman.sprites['front_default']} alt={data.props.pokeman.name} />
</div>