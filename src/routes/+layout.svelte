<script>
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Navbar from "../components/Navbar.svelte";
  import Sidebar from "../components/sidebar/Sidebar.svelte";
  import 'katex/dist/katex.min.css'
</script>

<Navbar />
<div class="grid grid-cols-5">
    <Sidebar />
    <div class="col-span-4 py-3 px-5">
        <slot/>
    </div>
</div>
<Footer/>


