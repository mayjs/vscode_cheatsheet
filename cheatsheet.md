# VSCode keys cheat sheet
<input id="searchbar" type="text" oninput="search()">
<div class="container">

<section class="important">

# Navigation
| Binding           | Effect           |
--------------------|-------------------
| C-P               | Fuzzy open file |
| C-Tab             | Goto previous file |
| C-T               | Fuzzy goto symbol in workspace |
| C-S-O             | Fuzzy goto symbol in file |
| C-F               | Find selection or word |
| A-Left; A-Right   | Go back or forward |

</section>


<section class="important">

# Quick selection
| Binding   | Effect           |
------------|-------------------
| S-A-Right | Expand selection |
| S-A-Left  | Shrink selection |
| C-L       | Select full line; expand to next line |
| C-D       | Select next occurance of word under cursor |

</section>
<section class="important">

# Window Navigation
| Binding       | Effect           |
----------------|-------------------
| C-B           | Toggle Side Bar |
| C-0           | Focus Side Bar |
| C-K C-Arrow   | Focus editor group in arrow direction |

</section>

<section class="medium">

# Quick Copying and Deleting
| Binding   | Effect           |
------------|-------------------
| C-C       | Copy entire line if nothing is selected |
| C-X       | Cut entire line if nothing is selected  |
| C-S-K     | Delete all lines that contain part of the selection |

</section>

<section class="medium">

# Integrated Terminal / Panel
| Binding   | Effect           |
------------|-------------------
| C-Ö       | Toggle Terminal |
| <span class="custom">C-S-J</span>     | <span class="custom">Toggle maximized Panel</span> |
| C-S-Ö     | New Terminal |

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


<section class="low">

# Window Management
| Binding   | Effect           |
------------|-------------------
| C-A-Arrow | Move editor to group in arrow direction |
| C-K Arrow | Move editor in arrow direction |
| C-^       | Split editor vertical |
| C-W       | Close editor |

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