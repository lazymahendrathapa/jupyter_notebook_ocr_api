To run api

jupyter kernelgateway --KernelGatewayApp.api='kernel_gateway.notebook_http' --KernelGatewayApp.seed_uri='main.ipynb'

To get the result

curl -d '{"image":"main.png"}' -H "Content-Type: application/json" -X POST http://localhost:8889/ocr
