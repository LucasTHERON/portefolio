<script>
    import Datas from './projets/test.json';

    let projetsArray = [];
    projetsArray.push(Datas);
    console.log(projetsArray[0][0].Name);
</script>

<h1>Projets</h1>
<hr>
<p>{#each projetsArray as data}
    <p>{data[0][0]}</p>
{/each}</p>
<hr>