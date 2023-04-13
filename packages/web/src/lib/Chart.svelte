<script>
    /*
wasm charts built in rust, rendering with webgl, multithreaded with rayon
capable of handling any data you send at it, as fast as native desktop application
example is built with vite and svelte
    */
    import init, { render_web_gl } from "vite-wasm-functions";
    init().then(() => {
        render_web_gl("canvas");
    });
</script>

<canvas id="canvas" width={400} height={400}></canvas>