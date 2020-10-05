    ### give input into input fiels that will automaticlt changed :

    <!DOCTYPE html>
    <html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
        <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
    </head>


    <body>

        <div id="app">
            <input type="text" v-on:input="changedfield">
            <p>{{ title }}</p>
        </div>

    </body>

    </html>



    <script>

        var x= new Vue({

            el: '#app',
            data: {

                title: "hello world"
            },
            methods: {

                changedfield: function (event) { // event object is created by vanila js
                    this.title = event.target.value;

                }
            }




        });
    </script>
