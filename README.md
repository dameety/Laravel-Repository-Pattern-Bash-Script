##What?
A simple bash script to scaffold repository pattern for your model, with controller and including it in service provider.

## How to use
Add the file to the root of your Laravel project directory and type this:

```
./repositorypattern.sh
```

In cases where you're going to use it on an online development environment, you need to assign permission to make the script executable, type this and press enter:

```
chmod +x ioc.sh
```

## What it does
After running the bash script, you will be prompted for a module name. After that input, the following is performed as a result of that:
- A Laravel model is created in the **app** directory.
- A migration file is created with the module name in **database/migrations**.
- A Service provider is created in **app/Providers** and registered inside **config/app.php** under the **providers** section.
- A Laravel Controller is created for you in **app/Http/Controllers** which implements all CRUD methods with necessary Dependency Injections.
- A Repositories directory which houses your repository files is created in the **app** directory.
- A **modulename** repository interface file and eloquent **modulename** file is created inside **app/Repositories/module_name** directory.
- The **modulename** repository interface and eloquent **modulename** are bound inside the respective Service Providers.

## Credits
- [Ohssie](https://github.com/Ohssie/laravel-IOC-module)
