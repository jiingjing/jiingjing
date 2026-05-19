<h2> Hi, I'm Jing! :sunny: </h2>

<div align="center">
<p><em>Maths, Stats and DS @ UoB :bathtub: 
</br>Placement @ <a href="https://www.crick.ac.uk/about-us">The FCI</a> :dna: 
</em></p>

[![Rooms.xyz: jing](https://img.shields.io/badge/-jing@Rooms-pink?style=flat-square&logoColor=white&link=https://rooms.xyz/jing)](https://rooms.xyz/jing)
[![GitHub Jing](https://img.shields.io/github/followers/jing?label=follow&style=social)](https://github.com/jiingjing)

</div>

---

<h3> About me :dog: </h3>

```python
class AboutMe:
    """
    A class that represents a personal profile and prints a simple introduction.
    """

    def __init__(self):
        self.name = "Jing"
        self.role = "student"
        self.programming_languages = ["Python", "R", "SQL", "JavaScript", "Lua"]
        self.pronouns = "she/her"
        self.hobbies = ["coding", "piano", "crochet"]

    def list_to_text(self, item_list):
        """
        Converts a list of items into a readable text string.

        Args:
            item_list (list[str]): A list of strings to join together.

        Returns:
            str: A single string where items are separated by commas,
                 with the last item joined using ", and ".
        """
        first_items = item_list[:-1]  # all items in list except last item
        text_list = ", ".join(first_items)  # join items with commas

        last_item = item_list[-1]  # last item in list
        text_list = ", and ".join(
            [text_list, last_item]
        )  # join last item to others with 'and'
        return text_list

    def introduction(self):
        """
        Prints a short self-introduction using stored profile attributes.

        Args:
            None

        Returns:
            None: This method prints text directly.
        """
        programming_languages_text = self.list_to_text(self.programming_languages)
        hobbies_text = self.list_to_text(self.hobbies)
        print(
            f"Hey, I'm a {self.role} called {self.name} ({self.pronouns}). "
            f"I code in {programming_languages_text}. I enjoy {hobbies_text}."
        )


me = AboutMe()
me.introduction()
```
