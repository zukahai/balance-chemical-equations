# <p align="center">API PTHH</p>
<p align="center"> <img src="https://github.com/zukahai/HaiZuka/blob/master/Images/balance-chemical-equations_2.png" alt="bg" /> </p>

1. Use API
```http
POST https://api-balance-chemical-equations.herokuapp.com/api/v1/pthh
data: 
{
   "pthh": "H2 + O2 = H2O"
}
```
Example with jquery javascript
```bash
   $.ajax({
       url: 'https://api-balance-chemical-equations.herokuapp.com/api/v1/pthh',
       type: 'POST',
       data: {
           "pthh": "H2 + O2 = H2O"
       },
       dataType: 'json',
       success: function(data, status, errors) {
            console.log(data);
           //solve data
       },
       error: function(data, status, errors) {
           console.log(errors);
       }
   })
```
2. Data JSon
```bash
{
    "message": "ok",
    "result": {
        "success": true,
        "input": "Ca(OH)2+O2=CaCO3+H2",
        "left": [
            "Ca(OH)2",
            "O2"
        ],
        "right": [
            "CaCO3",
            "H2"
        ],
        "element": {
            "Ca": 2,
            "O": 6,
            "H": 4
        },
        "data": {
            "dataLeft": {
                "Ca(OH)2": {
                    "Ca": 1,
                    "O": 2,
                    "H": 2
                },
                "O2": {
                    "O": 2
                }
            },
            "dataRight": {
                "CaCO3": {
                    "Ca": 1,
                    "C": 1,
                    "O": 3
                },
                "H2": {
                    "H": 2
                }
            }
        },
        "result": {
            "resultLeft": {
                "Ca(OH)2": 2,
                "O2": 1
            },
            "resultRight": {
                "CaCO3": 2,
                "H2": 2
            }
        },
        "text": "2Ca(OH)2 + O2 = 2CaCO3 + 2H2"
    }
}
```
<p align="center">
<a href="https://www.buymeacoffee.com/HaiZuka"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=HaiZuka&button_colour=5F7FFF&font_colour=ffffff&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00"></a>
</p>
Follow github.
<p align="center"> <img src="https://github.com/zukahai/Confess-Crush/blob/main/imagesGithub/follow.png" alt="bg" /> </p>

Follow me: https://github.com/zukahai
