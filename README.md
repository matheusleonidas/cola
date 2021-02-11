<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <title>Colas</title>
    <meta charset="utf-8" />
  </head>
  <body>
    <div class="hello">
    <img src="./estrutura.jpg" alt="Foto da estrutura de pastas" width="500" height="600">

      <h1>
        Isso é uma cola para quando eu precisar criar projetos com nodejs.
      </h1>
      <h3>Plugins do vscode</h3>

      <p>DotENV ESLint Prettier</p>

      <h3>Iniciar a aplicação</h3>

      <p>yarn init -y</p>

      <h3>Instalar typescript como dependencia</h3>

      <p>yarn add typescript ts-node-dev @types/node -D</p>

      <h3>Criar tsconfig.json</h3>

      <p>
        yarn tsc --init --rootDir src --outDir build --esModuleInterop
        --resolveJsonModule --lib es6 --module commonjs --allowJs true
        --noImplicitAny true
      </p>

      <h3>Isso deve ficar dentro do arquivo tsconfig.json</h3>
      <p>
        { "compilerOptions": { /* Visit https://aka.ms/tsconfig.json to read
        more about this file */ /* Basic Options */ // "incremental": true, /*
        Enable incremental compilation */ "target": "es5", /* Specify ECMAScript
        target version: 'ES3' (default), 'ES5', 'ES2015', 'ES2016', 'ES2017',
        'ES2018', 'ES2019', 'ES2020', or 'ESNEXT'. */ "module": "commonjs", /*
        Specify module code generation: 'none', 'commonjs', 'amd', 'system',
        'umd', 'es2015', 'es2020', or 'ESNext'. */ // "lib": ["es6"], /* Specify
        library files to be included in the compilation. */ "allowJs": true, /*
        Allow javascript files to be compiled. */ // "checkJs": true, /* Report
        errors in .js files. */ // "jsx": "preserve", /* Specify JSX code
        generation: 'preserve', 'react-native', or 'react'. */ // "declaration":
        true, /* Generates corresponding '.d.ts' file. */ // "declarationMap":
        true, /* Generates a sourcemap for each corresponding '.d.ts' file. */
        // "sourceMap": true, /* Generates corresponding '.map' file. */ //
        "outFile": "./", /* Concatenate and emit output to single file. */
        "outDir": "./build", /* Redirect output structure to the directory. */
        "rootDir": "./src", /* Specify the root directory of input files. Use to
        control the output directory structure with --outDir. */ // "composite":
        true, /* Enable project compilation */ // "tsBuildInfoFile": "./", /*
        Specify file to store incremental compilation information */ //
        "removeComments": true, /* Do not emit comments to output. */ //
        "noEmit": true, /* Do not emit outputs. */ // "importHelpers": true, /*
        Import emit helpers from 'tslib'. */ // "downlevelIteration": true, /*
        Provide full support for iterables in 'for-of', spread, and
        destructuring when targeting 'ES5' or 'ES3'. */ // "isolatedModules":
        true, /* Transpile each file as a separate module (similar to
        'ts.transpileModule'). */ /* Strict Type-Checking Options */ "strict":
        true, /* Enable all strict type-checking options. */ "noImplicitAny":
        true, /* Raise error on expressions and declarations with an implied
        'any' type. */ // "strictNullChecks": true, /* Enable strict null
        checks. */ // "strictFunctionTypes": true, /* Enable strict checking of
        function types. */ // "strictBindCallApply": true, /* Enable strict
        'bind', 'call', and 'apply' methods on functions. */
        "strictPropertyInitialization": false, /* Enable strict checking of
        property initialization in classes. */ // "noImplicitThis": true, /*
        Raise error on 'this' expressions with an implied 'any' type. */ //
        "alwaysStrict": true, /* Parse in strict mode and emit "use strict" for
        each source file. */ /* Additional Checks */ // "noUnusedLocals": true,
        /* Report errors on unused locals. */ // "noUnusedParameters": true, /*
        Report errors on unused parameters. */ // "noImplicitReturns": true, /*
        Report error when not all code paths in function return a value. */ //
        "noFallthroughCasesInSwitch": true, /* Report errors for fallthrough
        cases in switch statement. */ // "noUncheckedIndexedAccess": true, /*
        Include 'undefined' in index signature results */ /* Module Resolution
        Options */ "moduleResolution": "node", /* Specify module resolution
        strategy: 'node' (Node.js) or 'classic' (TypeScript pre-1.6). */
        "baseUrl": ".", /* Base directory to resolve non-absolute module names.
        */ // "paths": {}, /* A series of entries which re-map imports to lookup
        locations relative to the 'baseUrl'. */ // "rootDirs": [], /* List of
        root folders whose combined content represents the structure of the
        project at runtime. */ // "typeRoots": [], /* List of folders to include
        type definitions from. */ // "types": [], /* Type declaration files to
        be included in compilation. */ // "allowSyntheticDefaultImports": true,
        /* Allow default imports from modules with no default export. This does
        not affect code emit, just typechecking. */ "esModuleInterop": true, /*
        Enables emit interoperability between CommonJS and ES Modules via
        creation of namespace objects for all imports. Implies
        'allowSyntheticDefaultImports'. */ // "preserveSymlinks": true, /* Do
        not resolve the real path of symlinks. */ // "allowUmdGlobalAccess":
        true, /* Allow accessing UMD globals from modules. */ /* Source Map
        Options */ // "sourceRoot": "", /* Specify the location where debugger
        should locate TypeScript files instead of source locations. */ //
        "mapRoot": "", /* Specify the location where debugger should locate map
        files instead of generated locations. */ // "inlineSourceMap": true, /*
        Emit a single file with source maps instead of having a separate file.
        */ // "inlineSources": true, /* Emit the source alongside the sourcemaps
        within a single file; requires '--inlineSourceMap' or '--sourceMap' to
        be set. */ /* Experimental Options */ "experimentalDecorators": true, /*
        Enables experimental support for ES7 decorators. */
        "emitDecoratorMetadata": true, /* Enables experimental support for
        emitting type metadata for decorators. */ /* Advanced Options */
        "resolveJsonModule": true, /* Include modules imported with '.json'
        extension */ // "skipLibCheck": true, /* Skip type checking of
        declaration files. */ "forceConsistentCasingInFileNames": true, /*
        Disallow inconsistently-cased references to the same file. */ },
        "exclude": [ "node_modules", "build" ], "include": [ "src/**/*" ] }
      </p>

      <h3>Arquivo .gitignore</h3>
      <p>
        .idea/ .vscode/ node_modules/ build/ temp/ .env coverage ormconfig.json
        dist uploads/* !uploads/.gitkeep
      </p>

      <h3>Compilar o typescript</h3>
      <p>yarn tsc</p>

      <h3>Incluir no arquivo "package.json"</h3>
      <p>
        "scripts": { "dev": "ts-node-dev --inspect --transpile-only
        --ignore-watch node_modules src/server.ts" }
      </p>
      <h3>Executar o servidor</h3>
      <p>yarn dev</p>

      <h3>.editorconfig</h3>
      <p>
        root = true [*] indent_style = space indent_size = 2 charset = utf-8
        trim_trailing_whitespace = true insert_final_newline = true end_of_line
        = lf
      </p>
      <h3>Instalação do ESLint no projeto</h3>
      <p>
        yarn add -D eslint @typescript-eslint/parser
        @typescript-eslint/eslint-plugin
      </p>
      <h3>.eslintrc</h3>
      <p>
        { "root": true, "parser": "@typescript-eslint/parser", "plugins": [
        "@typescript-eslint" ], "extends": [ "eslint:recommended",
        "plugin:@typescript-eslint/eslint-recommended",
        "plugin:@typescript-eslint/recommended" ] }
      </p>
      <h3>.eslintignore</h3>
      <p>node_modules dist build /*.js</p>
      <h3>add script no package.json</h3>
      <p>
        "scripts": { "test": "echo \"Error: no test specified\" &amp;&amp; exit
        1", "dev": "ts-node-dev --inspect --transpile-only --ignore-watch
        node_modules src/server.ts", "lint": "eslint . --ext .ts" }
      </p>
      <h3>executar o lint</h3>
      <p>yarn lint</p>
      <h3>Regras do .eslintrc</h3>
      <p>
        { "root": true, "parser": "@typescript-eslint/parser", "plugins": [
        "@typescript-eslint" ], "extends": [ "eslint:recommended",
        "plugin:@typescript-eslint/eslint-recommended",
        "plugin:@typescript-eslint/recommended" ], "rules": { "no-console":
        "warn" } }
      </p>
      <h3>correção automatica (Outro script)</h3>
      <p>
        "scripts": { "test": "echo \"Error: no test specified\" &amp;&amp; exit
        1", "dev": "ts-node-dev --inspect --transpile-only --ignore-watch
        node_modules src/server.ts", "lint": "eslint . --ext .ts", "lint-fix":
        "eslint . --ext .ts --fix" }
      </p>
    </div>

  </body>
</html>

<style>
  div {
    text-align: center;
  }
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  p {
    color: red;
  }
</style>
