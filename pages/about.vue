<template>
    <div>
        <h2>About site</h2>
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
