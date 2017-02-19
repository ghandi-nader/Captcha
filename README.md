# Captcha


HTML example:
```
<div id="captcha"></div>
<button>generate</button>
```
```
Javascript example:

        $(function () {

            var captcha = new CAPTCHA({
                selector: '#captcha',
                width: 400,
                height: 200,
                onSuccess: function () { alert('Correct!'); },
               
            });
            
            $('button').on('click', function() {
            generate();
            })

            function generate() {
            	captcha.generate();
            }
            generate();

        });
```
