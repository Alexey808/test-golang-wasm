
# Тест запуска golang во frontend  

Источник: https://www.sitepen.com/blog/compiling-go-to-webassembly  


**Копиляция go файла**    
```
GOOS=js GOARCH=wasm go build -o main.wasm
```

**Копирование wasm файла для подключения скрипта в html**  
```
cp "$(go env GOROOT)/misc/wasm/wasm_exec.js" .
```