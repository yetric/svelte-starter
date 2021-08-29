<script>
    import { Router, Link, Route } from "svelte-navigator";
    import Home from "./routes/Home.svelte";
    import NotFound from "./routes/NotFound.svelte";
    import About from "./routes/About.svelte";
</script>

<Router>
    <nav>
        <Link to="/">Home</Link>
        <Link to="/about">About</Link>
        <Link to="/fsdfsdf">Non existing</Link>
    </nav>
    <div>
        <Route path="/" component={Home} />
        <Route path="about" component={About} />
        <Route component={NotFound} />
    </div>
</Router>
