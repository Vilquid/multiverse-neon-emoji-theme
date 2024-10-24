# multiverse-neon-emoji-theme

It's a fork of the multiverse-neon theme (Oh My Posh) which replace the arrow by sad emojis.

## Random

If you don't know which theme you need, you can download all from the Oh My Posh repo and move them to `/usr/local/share/oh-my-posh/prompt-themes/`.
This code will change your prompt whith a new theme on each new bash.

```sh
prompt_theme="$(find /usr/local/share/oh-my-posh/prompt-themes/ -type f | shuf -n 1)"
echo Thème utilisé : $(basename $prompt_theme)
echo "Commande pour supprimer le thème : rm $prompt_theme"
PROMPT_COMMAND="echo -ne '\n'; ${PROMPT_COMMAND}"
eval "$(oh-my-posh init bash --config $prompt_theme)"
```
