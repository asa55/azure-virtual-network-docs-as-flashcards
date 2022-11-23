# azure-vnet-docs-as-flashcards

## About this repository

Docs are boring, but very important.

If you want to learn anything fast, rote memorization is an important step in the process. Flashcards are one great way to pound basic bits of information into your brain, and retain massive volumes of information. Anki by far the most popular free and open-source flashcard app around, available for both desktop and mobile. The `azure-vnet-docs-as-flashcards` project helps me author and build Anki-compatible flashcard deck that you can build and download here on GitHub, or browse to from within the Anki application for download.

You and your team need a solid footing, and to speak the same technical lingo. If you or your team are trying to learn or onboard others as quickly and efficiently as possible, flashcards are in my biased opinion the absolute best approach to start with. It's critically important to have an understanding of what you're doing before you go off and try to use the technologies or some of the more nuanced features.

This is exactly where `*-docs-as-flashcards` comes in. I've taken the documentation and converted the critical information into a flashcard format, so that you and your team can study-up as quickly and efficiently as possible, then go off and confidently use these technologies to achieve what you've set out to achieve.

See the Notes section to understand how you can access the flashcards defined here.

## Notes

- This project leverages v2.0.0 of [`md2apkg-run`](https://github.com/asa55/md2apkg-run) to build Anki-compatible flashcard deck out of the `.md` flashcard definition files underneath the `Deck/` folder.
- Tags are automagically applied to the flashcards according to the folder hierarchy.
- The folder hierarchy in this project, and hence the flashcard tags, align with the [Azure VNET documentation here](https://docs.microsoft.com/en-us/azure/virtual-network/)
- Usage notes can be found in the [`md2apkg-run`](https://github.com/asa55/md2apkg-run) project readme.
- When I'm ready to release these notes, I'll put a successful build somewhere convenient and document that decision here. If you're reading this, the flashcards are coming along but I'm not at the point where I'm ready to tag a full release just yet.
- All of the flashcards in this deck are drawn from the official documentation at `learn.microsoft/azure/virtual-network`
  - Not all of the official documentation at `learn.microsoft/azure/virtual-network` is included in these flashcards
  - Project status is located on the project board. Issues are organized in a way that aligns with the Azure official documentation structure
- If you want to help influence what I add next, consider going to the appropriate issue and leaving a :+1: and/or a comment
  - If you really like the project and want to see more, faster, let me know. Once these flashcards reach a minimum level of maturity, I'll consider setting up a dono button or a link to my Patreon
- Lastly, I don't plan on stopping with VNET docs. I'll add more flashcard decks (to other repos on my GitHub account) related to Azure and technologies within and surrounding the .NET ecosystem. Keep an eye out for these
