<script>
    import { Router, Link, Route } from "svelte-navigator";
    import Home from "./routes/Home.svelte";
    import NotFound from "./routes/NotFound.svelte";
</script>

<Router>
    <nav>
        <Link to="/">Home</Link>
        <Link to="/about">About</Link>
    </nav>
    <div>
        <Route path="/">
            <Home />
        </Route>
        <Route component={NotFound} />
    </div>
</Router>
