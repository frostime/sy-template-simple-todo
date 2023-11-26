## Past month
{: id="20230524160202-8v1bgo8"}

{{SELECT * from blocks_esc_newline_WHERE `type` = &quot;l&quot; AND `subtype` = &quot;t&quot;_esc_newline_AND `created` &gt;= strftime('%Y%m%d%H%M%S', datetime('now', '-1 month')) _esc_newline_AND markdown REGEXP &quot;\* \[ \] \S+&quot;_esc_newline_AND `parent_id` not in (_esc_newline_  select `id` from blocks where `subtype` = &quot;t&quot;_esc_newline_)_esc_newline_ORDER BY `created` DESC}}
{: breadcrumb="true" custom-heading-mode="0" id="20230524160301-vtfzwvj" style="height: 3447px;"}

{: id="20230524160301-j47gnwx"}

## Past three months
{: id="20230524160211-rrx68qi"}

{{SELECT * from blocks_esc_newline_WHERE `type` = &quot;l&quot; AND `subtype` = &quot;t&quot;_esc_newline_AND `created` &gt;= strftime('%Y%m%d%H%M%S', datetime('now', '-3 month'))_esc_newline_AND `created` &lt; strftime('%Y%m%d%H%M%S', datetime('now', '-1 month')) _esc_newline_AND markdown REGEXP &quot;\* \[ \] \S+&quot;_esc_newline_AND `parent_id` not in (_esc_newline_  select `id` from blocks where `subtype` = &quot;t&quot;_esc_newline_)_esc_newline_ORDER BY `created` DESC}}
{: style="height: 4921px;" breadcrumb="true" id="20230524160225-slnhrii"}

{: id="20230524160636-as4etti"}

## Past six months
{: id="20230524160643-eeovfkl"}

{{SELECT * from blocks_esc_newline_WHERE `type` = &quot;l&quot; AND `subtype` = &quot;t&quot;_esc_newline_AND `created` &gt;= strftime('%Y%m%d%H%M%S', datetime('now', '-6 month'))_esc_newline_AND `created` &lt; strftime('%Y%m%d%H%M%S', datetime('now', '-3 month')) _esc_newline_AND markdown REGEXP &quot;\* \[ \] \S+&quot;_esc_newline_AND `parent_id` not in (_esc_newline_  select `id` from blocks where `subtype` = &quot;t&quot;_esc_newline_)_esc_newline_ORDER BY `created` DESC}}
{: breadcrumb="true" id="20230524160651-i7bqrut" style="height: 261px;"}

{: id="20230524160700-m8qjqi3"}

## Past year
{: id="20230804174147-fsrbyox"}

{{SELECT * from blocks_esc_newline_WHERE `type` = &quot;l&quot; AND `subtype` = &quot;t&quot;_esc_newline_AND `created` &gt;= strftime('%Y%m%d%H%M%S', datetime('now', '-1 year'))_esc_newline_AND `created` &lt; strftime('%Y%m%d%H%M%S', datetime('now', '-6 month')) _esc_newline_AND markdown REGEXP &quot;\* \[ \] \S+&quot;_esc_newline_AND `parent_id` not in (_esc_newline_  select `id` from blocks where `subtype` = &quot;t&quot;_esc_newline_)_esc_newline_ORDER BY `created` DESC}}
{: breadcrumb="true" custom-heading-mode="0" id="20231116221529-8ztjipx" style="height: 496px;"}

{: id="20230812222541-91mv9x5"}

## Further past
{: id="20230815001126-hfxvhqs"}

{{SELECT * from blocks_esc_newline_WHERE `type` = &quot;l&quot; AND `subtype` = &quot;t&quot;_esc_newline_AND `created` &lt; strftime('%Y%m%d%H%M%S', datetime('now', '-1 year'))_esc_newline_AND markdown REGEXP &quot;\* \[ \] \S+&quot;_esc_newline_AND `parent_id` not in (_esc_newline_  select `id` from blocks where `subtype` = &quot;t&quot;_esc_newline_)_esc_newline_ORDER BY `created` DESC}}
{: id="20231121162400-ir44do5" style="height: 38px;"}

{: id="20231121162414-kw2vopk"}
