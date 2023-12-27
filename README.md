This is configured docker file of the really cool github repo: https://github.com/rsxdalv/tts-generation-webui

You should use this in Portainer by adding a new stack and cloning the repo.
OR
You can cut and paste the yaml file into a new stack using the web editor (recommended if you need to alter a port or volume binding)

Volume bindings keep models persistent, which is the main change. Port number is also changed.

IMPORTANT: If you go into the WebUI settings and make ANY changes, you MUST set the port number to 7860 or you'll brick your image.
Remember, you're pointing 7840 on your host to container 7860. The Settings in the WebUi defaults to 0 or port 80, so you have to change it back.
