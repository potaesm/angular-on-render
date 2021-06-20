# AngularOnRender
## Configuration
1. Create [_redirects](src/_redirects) file in [src](src) directory
    - [_redirects](src/_redirects)
    ```bash
    /*    /index.html    200
    ```
2. Add [_redirects](src/_redirects) into build assets in [angular.json](angular.json) file
    - [angular.json](angular.json)
    ```json
    {
        "projects": {
            "architect": {
                "build": {
                    "options": {
                        "assets": [
                            "src/_redirects"
                        ]
                    }
                }
            }
        }
    }
    ```
3. Move all assets to [src/assets](src/assets) e.g. [favicon.ico](src/assets/favicon.ico)
4. Render dashboard settings
    - Name
    ```bash
    AppName
    ```
    - Build Command
    ```bash
    ng build
    ```
    - Publish directory
    ```bash
    dist/app-name
    ```