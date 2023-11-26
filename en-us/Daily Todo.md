.action{$datestr_sy := now | date "20060102"}

> Unsolved
> {{select B.* from blocks as B join attributes as A_esc_newline_on B.id = A.block_id_esc_newline_where B.markdown like '%[ ]%' and A.name='custom-daily-todo' and A.value < '.action{$datestr_sy}';}}
> {: breadcrumb="true"}
{: custom-b="warn" breadcrumb="true" custom-heading-mode="0" }


> Daily Todo
>
> {{{col
> * High-priority
>
>   * [ ] TODO
>   {: custom-daily-todo=".action{$datestr_sy}" }
> {: id="" }
>
>
> * Low-priority
>
>   * [ ] TODO
>   {: custom-daily-todo=".action{$datestr_sy}" }
> {: id="" }
> }}}
{: custom-b="bell" breadcrumb="true" custom-heading-mode="0" }
