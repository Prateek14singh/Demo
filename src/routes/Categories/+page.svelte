<script>
	import '../../Design.css';
	import Data from '../../Data.json';
</script>

<nav class="bg-white sticky top-0 drop-shadow-md items-center">
	<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 flex justify-between py-4">
		<a href="./"><img
			src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMQAAAAuCAMAAABAp0a9AAAAUVBMVEUAAAAAbTUAbDUAbTMAbTMAbTEAbTIAbjUAbTIAbTIAbTIAbTIAbTIAbTIAbTIAbjUAbjAAbjEAbTEAbTIAbTIAbTIAbTMAbTIAbTIAbTMAbTJazT9DAAAAGnRSTlMAFQjQvUmzJtruiOT2aFwdNy5AlKhTdMSefipyKHAAAAZBSURBVGje1ZqLcqMgFIbDAQVERPHO+z/oaiJ3NW3Tndn9p502SUW+c5fp4ydCzeM/F6UPNQB06vH/is5YaYZaMcDjn9E6SadpXatNqxz1pZ1VSZDkbYf7UwgoRl0U13xIaz2Ov81vzsQFLqfuZIsKHgg9SlM90PabyjfTYS6EkI8rTUIIzuhfhvASS5tBjEO5yr42vJJVueh8Oc3NJoyughE/baQfvyE0NQmEwE8JHjpkhZSiW7i9oKInUTGaXbW8csRr3fE3knPCpooh6gmeQl1TzR6kpLmt8euT7nRpaZ4icJ5Q2DJ+KGgrsS00JRAyCpraUsz0LGIWgy8yvzqWa+4QTfUhgj7iQeYQXiCFpSBZeBc1oeIiN2GwLoSzIMbHp8snCH6deswgImlmKZZ0O4vRm0nX83iZjbkOe+ks8wmCvwsvMohYhTDnkaH5FomwMHpRfQ4N6MKAtnp9IETuIbwmd0cVLbA8Axr2H7laVxPq4qQ0WTH6GUT5VQg0m0PRR90IxxB4ltraOA2QO8JK6M8S+y1Ebjjydec3HqJuT9a7zBhAiioE93sHOP5gOJbRbyFacbIdQE5nt1yNVVYRABsvmQxUFWGcc1yuLYTvd1QpRTv0fDH25VxsPxVCFmIEQAjuIMDF0xpEU+VF80v6sN/H7VDWxquKWu8c+G8JrmpqwRgTfL//+LTBBjExTKx5yTKUpLMQp91pMXnRR60XOs04P7j0mUmYyBoFmrCJxLTPMI/cPFcVrWunHvsewtcn9I0uNFTW5JwmjhByTs2iibHKS1cnDggb2myDmARj/LgBxpjhe4iR290oN/+1obJ4omIzssLOFUlpHxCJa8Vh17mfZFXWLpnSrlPZTGbbhlXXtYct5o7SroNbiII7jznfV6FkmtpdvW3BZ7fogvDeWweU1rfUvz83Cva1C+IuSzrz2nIHsQtIMmZaY59AaDdAaWfQSHA2iFcP5a6rovZEHmDTjLXuHr61K4s42TfI4dHkMmQh0HuINoUABLHQSRatQe4xGtCZ7Ra9SdoUGt0aPgeWMAZtPeCc1+INxHgHcdhN94nSKlu9WkDHfXH2jsAQ9JHmbgYm4CCsiNStlpP6NoQWSU7QYixCjQXKNzHuMMncVdh9uzl2uoPAyLLbDbhHzFuIerxJbKG+ONOQYxRoebRZKO3Oxrxw5a7PIXzzv4c48W/Dkz4BmZLF2d6PbOf2rigcjuZ+PMwZZne/bFr9McQUD6TdMJNUcx8GFOW2ePp0kk9HuPeZ7XYoQ1iZuYDA6ucQfRzAaGxyFZAM4rOKRpb9deFTnGLfKLyQlhWx2CGE6wc/hgASV9j3kt7Emvs6VNo2ZSu/e70LigXzeg+aoRl+G8JbbX6NwgoFUk4QV9gBwkKzUz1Tq0pSlWsbRXaiWDuAJYZQ34WQ+ehURxVmIuWZ5iYee5dsZhGB4WFIGsUojrSjWYn1Y0f5c4g+GmWgLc4VzP/EmtyWVaf+Is+0ZQDvJw9B8aee6Nh3T7qA2c05R2YZsEZjFSLu878DUUVNFxWX0hBUWNOET0F5a5PRw2txgA52czFE9ylEwaN5pMGXItQdDUbjS+NcIWiUaL5RrLGzFU4gmK0sP4PocDLCdfRSEFhZ6JOTgT6yjXcw9PFNKIshWvERRIu9198KggBkQZ7L3BG+ZYvOQnhKbRIIft+x5zsI1LCYAaoyF9m+9u+SNP40CNP8tKw/PefUQTgRiNJwhgOqfgOhrpod0MZNwBXYW7M7vVABp56X/ugmP1ccg6GWS1tvo0Qushkl7jbCruzithh3Nevgj309GLqXfS5LColiz5XhdJaRQSYbsepiEobHFXlMK3RaqCuIIHKJ3l8K7+QOR4ZsDubxceYQNQpprOr9jGGypWtsUXAoyuIl/GRW92MhG3QFgSsdhAV5o7KzER1DUJY9OSzRfA+V8RoQDBZJFAHi/sIruqzme7EWGM/zjJngnAvG8Pay7KdChZcsDL9Rs/uYDCVJKvXEmU7ewaQchu0vX6EAEltzTyg48Hg2n0Y8xXGRFcSVu4hp4EEV2qX2YyhKlTo7ikFvBa+zkOzS/L8nQCEEsCeZTZymH0jZS3qcbBHG5v718A6+E2XSVYkxLvuG/kP/2fCJ/gA4IBwj83FAYQAAAABJRU5ErkJggg=="
			alt="DMART"
		/></a>

		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="./About"
			>ABOUT US</a
		>
		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="./Categories"
			>CATEGORIES</a
		>
		<a class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center" href="/Social Outreach"
			>SOCIAL OUTREACH</a
		>
		<a
			class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center"
			href="./Partner with us">PARTNER WITH US</a
		>
		<div class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center">CAREERS</div>
		<div class="text-black font-bold py-4 px-2 hover:bg-green-100 text-center">FEEDBACK</div>
		<div class="flex justify-between text-lg font-bold py-4" />
	</div>
</nav>
<div class="font-bold underline underline-offset-4 justify-center flex my-4">Categories</div>
<div class="flex justify-around flex-wrap">
	{#each Data.categories as category}
		<div class=" rounded-xl border border-slate-300 w-1/5 my-2 ml-2">
			<img src={category.image} alt={category.name} class="w-full rounded-t-xl" />
			<h1 class="w-full opacity-70 bg-gray-700 mb-0 text-white rounded-b-xl">{category.name}</h1>
		</div>{/each}
</div>
<div class="bg-gray-600 flex justify-between text-white px-8 py-4 font-weight-600 mt-3">
	<span class="font-medium">Site map</span>
	<span class="font-medium">Privacy policy</span>
	<span class="font-medium">Terms Of Use</span>
	<span class="font-medium">Investor relations</span>
</div>
