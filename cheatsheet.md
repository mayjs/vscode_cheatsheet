# VSCode keys cheat sheet
<input id="searchbar" type="text" oninput="search()">
<div class="container">

<section class="important">

# Quick selection
| Binding   | Effect           |
------------|-------------------
| S-M-Right | Expand selection |
| S-M-Left  | Shrink selection |
| C-L       | Select full line; expand to next line |

</section>

</div>

<script>
    function search(e) {
        const term = document.getElementById("searchbar").value.toLowerCase();
        Array.from(document.getElementsByTagName("section")).forEach(section => {
            if(section.innerText.toLowerCase().includes(term)) {
                section.style.display = "block";
            } else {
                section.style.display = "none";
            }
        });
    }
</script>