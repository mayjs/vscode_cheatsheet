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

<section class="medium">

# Quick Copying and Deleting
| Binding   | Effect           |
------------|-------------------
| C-C       | Copy entire line if nothing is selected |
| C-X       | Cut entire line if nothing is selected  |
| C-S-K     | Delete all lines that contain part of the selection |

</section>

<section class="low">

# Code Folding
| Binding   | Effect           |
------------|-------------------
| C-K C--   | Close all folds except the selected block |
| C-K C-8   | Close all folds |
| C-K C-J   | Open all folds |
| C-K C-L   | Toggle fold |

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