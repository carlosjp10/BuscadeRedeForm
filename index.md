<html>
    <style>
        a {
            color:blue;
        }
    </style>

    <script src="https://unimedrp--dev.sandbox.my.salesforce-sites.com/lightning/lightning.out.js"></script>

    <div data-lightning-out="true"></div>

    <script>
        const appName = 'c:buscaDeRedeApp';
        const componentName = 'c:buscaDeRedeForm';
        const lightningEndpoint = 'https://unimedrp--dev.sandbox.my.salesforce-sites.com';
        const targetElement = document.querySelector("[data-lightning-out]");
        const componentAttributes = {

        };

        $Lightning.use(
            appName,
            function(){
                $Lightning.createComponent(
                    componentName,
                    componentAttributes,
                    targetElement,
                    function(cmp){
                        console.log('@cac funcionando');
                    }
                );
            },
            lightningEndpoint
        );
    </script>
</html>
