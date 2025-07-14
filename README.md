# Autobrace.vim
A simple Vim9.1 plugin that can simplify working with matching brackets and
quotes

## Usage
Just clone this repository into your Vim Package directory.

```sh
cd $HOME/.config/vim/pack/vim/start
git clone https://github.com/riturajborpujari/autobrace.vim
```

Restart Vim to see effect

## Features
1. Brackets and quotes are auto closed.
    

    When in `Insert` mode, typing the opening character of a bracket or quote
    (`(`, `{`, `[`, `<backtick>`, `"`, `'`) automatically inserts the relevant
    closing character after it. The cursor is placed back at the original 
    postion.

    Eg., typing `(` automatically inserts `)`
2. Auto escapes closing characters of brackets and quotes

    Typing closing bracket characters like `)`, `}`, `]`, and quote characters
    like `'`, `"`, and `<backtick>`, and escapes the input if the character is
    already present
3. Pressing `<Backspace>` key for deleting pairs need only one key press if the
   pairs are together.
   

   This works if the cursor inside the pair as well.

   Eg., typing `<Backspace>` after `{}` deletes both the characters together.
4. Pressing `<Return>` key immediately after a opening bracket will add a new
   line and move the closing character to another line below


   Eg., pressing `<Return>` key in the middle of `{}` will get you to something
   like, with cursor position as shown below
   ```
   {
       <Cursor>
   }
   ```

## Note
This work is a modification of the
[closepairs](https://www.vim.org/scripts/script.php?script_id=2373) script by
Edoardo Vacchi
