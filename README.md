To edit the entry file, open 'assembly/index.ts' in your editor of choice.
Create as many additional files as necessary and use them as imports.

To build the entry file to WebAssembly when you are ready, run:

  npm run asbuild

Running the command above creates the following binaries incl. their respective
text format representations and source maps:

  ./build/debug.wasm
  ./build/debug.wasm.map
  ./build/debug.wat

  ^ The debuggable WebAssembly module as generated by the compiler.
    This one matches your sources exactly, without any optimizations.

  ./build/release.wasm
  ./build/release.wasm.map
  ./build/release.wat

  ^ The optimized WebAssembly module using default optimization settings.
    You can change the optimization settings in 'package.json'.

To run the tests, do:

  npm test

The AssemblyScript documentation covers all the details:

  https://www.assemblyscript.org

Have a nice day!
