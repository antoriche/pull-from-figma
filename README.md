# pull-from-figma

this is a tool aiming to help developers to download and keep updated figma templates as react components  

## How to use
1. [Get an access token](https://www.figma.com/developers/api#access-tokens) on figma and store it in `FIGMA_TOKEN` env variable  
```export FIGMA_TOKEN=<YOUR_TOKEN>```
2. create a file `figma.json` with the following structure :  
```
{
    "ref":{
        "figma_id": "",
        "output": ""
    }
}
```
  - `ref` will be a reference to update this component
  - `figma_id` is your figma project id (you can find it in the project url www.figma.com/file/{id})
  - `output` is a javascript file the component will be written
3. run `npx pull-from-figma` with eventually `--ref=ref` to generate the files