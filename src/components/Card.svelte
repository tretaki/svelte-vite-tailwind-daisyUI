<script>
    export let cardTitle = "Card Title";
    export let cardText = "Card Text";
</script>

<div class="card w-96 bg-base-100 shadow-xl">
    <figure><slot /></figure>
    <div class="card-body">
        <h2 class="card-title">{cardTitle}</h2>
        <p>{cardText}</p>
        <div class="card-actions justify-end">
            <button class="btn btn-primary">Explore</button>
        </div>
    </div>
</div>
