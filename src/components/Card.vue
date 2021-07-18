<template>
    <div id="container">
        <div id="title-container">
            <h2 id="title">{{title}}</h2>
        </div>
        <div id="body-container">
            <p id="body">{{body}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name:'Card',
    props: {
        title: String,
        body: String
    },    
}
</script>

<style>
    :root {
         --gray-color: #CCCCCC;
    }
    
    #container {
        font-family: Arial;
        display:flex;
        flex-direction: column;
        height: 300px;
        width: 150px;
    }

    #title-container {
        flex-basis: 55px;
        display: flex;
        justify-content: flex-start;
        align-items: center;
        border-color: black;
        border-style: solid;
        border-width: 2px 2px 0px 2px;
    }

    #title {
        margin: auto 5px auto 5px;
        overflow-wrap: break-word;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 1; 
        -webkit-box-orient: vertical;
    }

    #body-container {
        flex-basis: 245px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color:var(--gray-color);
        border: 2px solid black;
    }
    
    #body { 
        margin: auto 2px auto 2px;
        font-size: 14px;
        text-align: center;
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 14; 
        -webkit-box-orient: vertical;
    }
</style>