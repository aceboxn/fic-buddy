# fic-buddy
Discord bot to pick and manage flash fic prompts.

## Commands

### Playing a Round

* `_play` - promptmaster chooses to start a round, players get 60 seconds to join before prompting begins (whoever issues this command automatically becomes the promptmaster)
* `_in` - player joins, can do so at any time during a round
* `_out` - player leaves the round

`_pick # letter @user` - promptmaster prompts a user to pick however many letters they want
`_pick # genre @user` - promptmaster prompts a user to pick however many genres they want (whump and fluff supported)
`_pick # number @user` - promptmaster prompts a user to pick the numbers to choose the prompts

At this point, definitions for each of the prompts display, and fics can be submitted.

`_fic TEST` - user submits their fic for the round, and _fic can be submitted a second time to provide a second half within the next 30 seconds

There is a countdown as each user submits, and after everyone submits, a round finished message appears.

`_end` - promptmaster can end a round prematurely (useful if a person never provides a response)

### Get Pinged for Each Round

`_remind` - always pings a user at the start of a flash fic round
`_stop` - removes the user from being reminded at the start of a flash fic round

### Stats for a Round

`_stats a` - see counts of all past prompt responses by letter
`_history [prompt]` - see all past fics for a given prompt

### Manage Available Prompts (promptmaster)

`_manage add [prompt word]` - promptmaster adds one to many prompts, separated by spaces; multi-word single prompts must be in quotes " "
`_manage delete [prompt word]` - promptmaster deletes one to many prompts, separated by spaces; multi-word single prompts must be in quotes " "
`_prompt update [prompt] genre [name]` - promptmaster updates the genre for a single prompt to whump or fluff; multi-word single prompts must be in quotes " "
