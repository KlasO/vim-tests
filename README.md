# vim-tests  
This repo contains my test files while learning vim.

This is my textbook: [Learn vimscript the hard way](https://learnvimscriptthehardway.stevelosh.com)  

Operator-Pending Mappings
=========================
onoremap ip( :<c-u>normal! F(vi(<cr> ; inside previous parentheses; this is my example
onoremap il( :<c-u>normal! F)vi(<cr> ; did not yet figure out why these two has the same result
onoremap al( :<c-u>normal! F)va(<cr>
onoremap an( :<c-u>normal! f)va(<cr>

onoremap ip{ :<c-u>normal! F{vi{<cr> 
onoremap il{ :<c-u>normal! F}vi{<cr> 
onoremap al{ :<c-u>normal! F}va{<cr>
onoremap an{ :<c-u>normal! f}va{<cr>

More Operator-Pending Mappings
==============================
onoremap ih :<c-u>execute "normal! ?^\[=-\]\\+$\r:nohlsearch\rkvg_"<cr>
onoremap ah :<c-u>execute "normal! ?^\[=-\]\\+$\r:nohlsearch\rg_vk0"<cr>

onoremap in@ :<c-u>execute "normal! /\S*@\w*\.\w*\r:nohlsearch\rviW"<cr>
did not figure out this one either; need to study regex more

Status Lines
============

