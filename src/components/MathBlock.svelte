<script>
    // @ts-nocheck
    
        import katex from 'katex'
        const render = n => katex.render(n.textContent, n)
    </script>
    <span class="block my-2">
        <span use:render><slot/></span>
    </span>
    