<script>
    import { Heading, P, A, Hr, Button } from "flowbite-svelte";
    import { base } from "$app/paths";
</script>

<Heading class="p-8" tag="h1">WebAssembly Reverse Engineering Challenge</Heading
>

<P class="px-8 py-4">
    This website contains hacking challenges involving reverse engineering of <A
        href="https://webassembly.org/">WebAssembly</A
    > programs.
</P>

<P class="px-8 py-4"
    >Levels are increasingly more difficult. Each one exposes a single function
    callable by Javascript: <code>hash()</code>. It returns the <A
        href="https://en.wikipedia.org/wiki/SHA-2">sha256</A
    > sum of a flag. The goal is to retrieve the flag's original value. All flags
    follow the <code>flag{"{"}...{"}"}</code> format. You can easily check if your
    guess is correct as you have access to the answer's hash.
</P>

<div class="basis-1/4 flex flex-col items-center justify-center">
    <Button href={`${base}/level1`} color="light"
        >Get started with level1!</Button
    >
</div>

<Hr />

<Heading class="p-8" tag="h2">Frequently asked questions</Heading>

<P class="px-8 py-4" weight="bold">Can I publish answers?</P>
<P class="px-8 py-4">Sure, I don't mind if you do!</P>

<P class="px-8 py-4" weight="bold">I found a bug and I'd like to report it</P>
<P class="px-8 py-4"
    >Feel free to <A href="https://github.com/juliendoutre/warec/issues"
        >open an issue</A
    > on the GitHub repository hosting this website source code 🙏</P
>

<P class="px-8 py-4" weight="bold">I'd like to propose a new challenge!</P>
<P class="px-8 py-4"
    >I definitely accept ideas for new levels! Please send me an email at
    jul.doutre@gmail.com.</P
>
