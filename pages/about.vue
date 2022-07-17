<template>
    <div id="main_about">
            <div class="container_about">
                <h2>About site</h2>
                <h4>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt, tempora itaque temporibus dolorum minima eum sapiente iste recusandae ipsa eius fugiat blanditiis necessitatibus nisi repudiandae ducimus ullam voluptas. Molestias aut quasi in, suscipit nam explicabo sit laudantium quo perferendis. Quos inventore molestiae cupiditate non dicta. Provident quod, recusandae facere eum sit expedita at alias perspiciatis. Dicta velit eveniet, veritatis aut commodi voluptates aliquid, quis molestias autem, exercitationem cum amet provident ab. Nobis veniam impedit cumque ad voluptas. Suscipit corrupti laboriosam quo, libero id cum. Voluptate corrupti velit ullam debitis officiis, consequuntur quisquam, minus ipsa dolores aspernatur cupiditate delectus magnam numquam?</h4>
            </div>
    </div>
</template>

<script>
export default {
  name: 'About',

    head(){
        return{
            title:"About page",
            meta:[
                {
                    hid:"discription",
                    name:"other discripation",
                    content:"this is a content for about page"
                }
            ],
            link:[
                 { 
                    rel: 'icon', type: 'icon', href: 'https://wallpapercave.com/w/wp2506795' 
                    
                },
            ]
        }
    }

}
</script>


<style lang="css">
    #main_about{
        height: 80vh;
        display: flex; justify-content: center; align-items: flex-start;
        flex-direction: column;
        user-select: none;
    }
    .container_about{
        width:70%;
        padding-left: 2rem;
    }
    .container_about h2{
        margin-bottom: 1.5rem;
        border-bottom: 1px solid gray;
        padding-bottom: 1rem;
    }
    .container_about h4{
        line-height: 1.5rem;
    }
</style>