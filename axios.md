
AXIOS POST

```
  <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
  const axios = require('axios');
  const url = "http://localhost:4000/test";

  const data = {"id1": '123', "id2": 456};

  const config = {
    headers: { //헤더를 추가해야 OPTION이라고 안뜬다.
       "content-type": "multipart/form-data",
       "content-type": "Application/json"
    }
  }

  axios.post(url, data, config);
  
 ```
 
 FETCH POST
 
 ```
  const option = {
    method: 'POST',
    header : {
      'accept' : 'app'
    },
    body : JSON.stringify({ //제이선으로 만듬
      name : 'junwon',
      age : 20
    })
  }
  
  fetch(url,option);

 
 ```
