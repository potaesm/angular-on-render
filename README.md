# AngularOnRender
## Configuration
1. Create ***_redirects*** file in ***src*** directory
    - _redirects
    ```bash
    /*    /index.html    200
    ```
2. Add _redirects into build assets in ***angular.json*** file
    - angular.json
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
3. Render dashboard settings
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