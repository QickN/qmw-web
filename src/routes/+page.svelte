<script>
	import { goto } from "$app/navigation";
</script>

<svelte:head>
    <title>QMW Solutions</title>
    <meta name="description" content="Innovative Technology Solutions by TraceValley" />
</svelte:head>

<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap">

<main>

    <section class="hero">
        <h1>QMW SOLUTIONS</h1>
        <p>we are engineers</p>
		<button on:click={() => goto('/about')}>learn more</button>
    </section>

	  

    <!-- Add your other sections like About, Services, Contact here -->

</main>


<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
		margin: 0;
	}

	h1 {
		width: 100%;
		font-weight: bold;
		font-size: 5rem;
		margin: 0;

	}

	p{
		font-style: italic;
		font-size: 1.3rem;
		margin: 0;
	}

	button {
		padding: 10px 20px;
        background-color: #B80000;
        color: white;
        border: none;
        border-radius: 7px;
        cursor: pointer;
        margin-top: 20px; /* Space between text and button */

	}

	button:hover{
		background-color: #FF9800;
	}


</style>
