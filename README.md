# Gutenberg Block Unit Test

Testing every core block — and every variation of every block — is no small task. That's why I built the Block Unit Test WordPress plugin. Deploy the Block Unit Test WordPress plugin and review every core Gutenberg block to ensure your theme fully supports Gutenberg. [Keep reading...](https://richtabor.com/gutenberg-block-unit-test/)

## Installation ##

1. Add the plugin respository to the composer.json
  
  ```json
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "threespot/block-unit-test",
        "version": "dev-master",
        "type": "wordpress-plugin",
        "dist": {
          "url": "https://github.com/Threespot/block-unit-test/archive/master.zip",
          "type": "zip"
        }
      }
    }
  ], 

  ```
2. Install the composer dependency
  ```
  composer require threespot/block-unit-test:dev-master
  ```
3. Activate the plugin via WordPress CLI
  ```
   wp plugin activate block-unit-test
  ```
4. You will find a new pages added with their titles prepended with `Test - `. Each of the core Gutenberg blocks will be added here for you to start testing.

## Development ##
1. Clone the GitHub repository: `https://github.com/that-plugin-company/block-unit-test.git`
2. Browse to the folder in the command line.
3. Run the `npm install` command to install the plugin's dependencies within a /node_modules/ folder.
4. Develop stuff.
5. Run the `build` gulp task to process build files and generate a zip.