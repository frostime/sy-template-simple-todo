.action{$datestr_sy := now | date "20060102"}

> 未完成
> {{select B.* from blocks as B join attributes as A_esc_newline_on B.id = A.block_id_esc_newline_where B.markdown like '%[ ]%' and A.name='custom-daily-todo' and A.value < '.action{$datestr_sy}';}}
> {: breadcrumb="true"}
{: custom-b="warn" breadcrumb="true" custom-heading-mode="0" }


> 今日 Todo
>
> {{{col
> * 高优先
>
>   * [ ] TODO
>   {: custom-daily-todo=".action{$datestr_sy}" }
> {: id="" }
>
>
> * 低优先
>
>   * [ ] TODO
>   {: custom-daily-todo=".action{$datestr_sy}" }
> {: id="" }
> }}}
{: custom-b="bell" breadcrumb="true" custom-heading-mode="0" }
