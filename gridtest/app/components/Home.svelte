<page>
    <actionBar title="Home" />
    <gridLayout columns="100, auto, *" rows="100, auto, *" backgroundColor="#3c495e">
        <label text={`counter = ${counter}`} row="0" col="0" backgroundColor="#4383b8"/>
        <label text="0,1" row="0" col="1" colSpan="2" backgroundColor="#1c486b"/>
        <label text="1,0" row="1" col="0" rowSpan="2" backgroundColor="#286290"/>
        <label text="1,1" row="1" col="1" backgroundColor="#4383b8"/>
        <label text="1,2" row="1" col="2" backgroundColor="#286290"/>
        <label text="2,1" row="2" col="1" backgroundColor="#1c486b"/>
        <button on:tap={handle} text="2,2" row="2" col="2" backgroundColor="#4383b8"/>
    </gridLayout>
</page>

<script>
  let counter = 0;
    function handle(){
      counter++; //
    }
    console.log('1111');

    if(counter === 5){
      [1,2,3].map(el=>{
        console.log(el)
        return el * 2;
      })
    }
</script>

