var obj = {}; 
obj[key] = 'value'; 
console.log(obj);

> 실행 결과 

[Running] node "c:\Dev\JAVA - class\11_JavaScript\01_lecture-source\02_variable\01_data-type\tempCodeRunnerFile.js"
c:\Dev\JAVA - class\11_JavaScript\01_lecture-source\02_variable\01_data-type\tempCodeRunnerFile.js:2
obj[key] = 'value'; 
    ^

ReferenceError: key is not defined // 키가 정의되지 않았다. 
    at Object.<anonymous> (c:\Dev\JAVA - class\11_JavaScript\01_lecture-source\02_variable\01_data-type\tempCodeRunnerFile.js:2:5)
    at Module._compile (node:internal/modules/cjs/loader:1256:14)
    at Module._extensions..js (node:internal/modules/cjs/loader:1310:10)
    at Module.load (node:internal/modules/cjs/loader:1119:32)
    at Module._load (node:internal/modules/cjs/loader:960:12)
    at Function.executeUserEntryPoint [as runMain] (node:internal/modules/run_main:81:12)
    at node:internal/main/run_main_module:23:47

Node.js v18.17.0

[Done] exited with code=1 in 0.088 seconds

-----------------------------------------------------------------

'Key'라는 변수가 정의되지 않았기 때문!
      따라서, obj에 새로운 속성을 추가할 수 없었던 것- 

      var obj = {};
      var key = 'someKey';
      obj[key] = 'value';
      console.log(obj);

      > 실행 결과 
    
      [Running] node "c:\Dev\JAVA - class\11_JavaScript\01_lecture-source\02_variable\01_data-type\tempCodeRunnerFile.js"
      { someKey: 'value' }

      [Done] exited with code=0 in 0.086 seconds

      
