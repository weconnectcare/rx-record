# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [drugs](#drugs)
    * [drugs_aggregate](#drugs_aggregate)
    * [drugs_aggregate_fields](#drugs_aggregate_fields)
    * [drugs_max_fields](#drugs_max_fields)
    * [drugs_min_fields](#drugs_min_fields)
    * [drugs_mutation_response](#drugs_mutation_response)
    * [gender_enum](#gender_enum)
    * [gender_enum_aggregate](#gender_enum_aggregate)
    * [gender_enum_aggregate_fields](#gender_enum_aggregate_fields)
    * [gender_enum_max_fields](#gender_enum_max_fields)
    * [gender_enum_min_fields](#gender_enum_min_fields)
    * [gender_enum_mutation_response](#gender_enum_mutation_response)
    * [patients](#patients)
    * [patients_aggregate](#patients_aggregate)
    * [patients_aggregate_fields](#patients_aggregate_fields)
    * [patients_max_fields](#patients_max_fields)
    * [patients_min_fields](#patients_min_fields)
    * [patients_mutation_response](#patients_mutation_response)
    * [prescription_item](#prescription_item)
    * [prescription_item_aggregate](#prescription_item_aggregate)
    * [prescription_item_aggregate_fields](#prescription_item_aggregate_fields)
    * [prescription_item_avg_fields](#prescription_item_avg_fields)
    * [prescription_item_max_fields](#prescription_item_max_fields)
    * [prescription_item_min_fields](#prescription_item_min_fields)
    * [prescription_item_mutation_response](#prescription_item_mutation_response)
    * [prescription_item_stddev_fields](#prescription_item_stddev_fields)
    * [prescription_item_stddev_pop_fields](#prescription_item_stddev_pop_fields)
    * [prescription_item_stddev_samp_fields](#prescription_item_stddev_samp_fields)
    * [prescription_item_sum_fields](#prescription_item_sum_fields)
    * [prescription_item_type_enum](#prescription_item_type_enum)
    * [prescription_item_type_enum_aggregate](#prescription_item_type_enum_aggregate)
    * [prescription_item_type_enum_aggregate_fields](#prescription_item_type_enum_aggregate_fields)
    * [prescription_item_type_enum_max_fields](#prescription_item_type_enum_max_fields)
    * [prescription_item_type_enum_min_fields](#prescription_item_type_enum_min_fields)
    * [prescription_item_type_enum_mutation_response](#prescription_item_type_enum_mutation_response)
    * [prescription_item_var_pop_fields](#prescription_item_var_pop_fields)
    * [prescription_item_var_samp_fields](#prescription_item_var_samp_fields)
    * [prescription_item_variance_fields](#prescription_item_variance_fields)
    * [prescriptions](#prescriptions)
    * [prescriptions_aggregate](#prescriptions_aggregate)
    * [prescriptions_aggregate_fields](#prescriptions_aggregate_fields)
    * [prescriptions_max_fields](#prescriptions_max_fields)
    * [prescriptions_min_fields](#prescriptions_min_fields)
    * [prescriptions_mutation_response](#prescriptions_mutation_response)
    * [subscription_root](#subscription_root)
  * [Inputs](#inputs)
    * [Boolean_comparison_exp](#boolean_comparison_exp)
    * [Int_comparison_exp](#int_comparison_exp)
    * [String_comparison_exp](#string_comparison_exp)
    * [drugs_bool_exp](#drugs_bool_exp)
    * [drugs_insert_input](#drugs_insert_input)
    * [drugs_obj_rel_insert_input](#drugs_obj_rel_insert_input)
    * [drugs_on_conflict](#drugs_on_conflict)
    * [drugs_order_by](#drugs_order_by)
    * [drugs_pk_columns_input](#drugs_pk_columns_input)
    * [drugs_set_input](#drugs_set_input)
    * [gender_enum_bool_exp](#gender_enum_bool_exp)
    * [gender_enum_enum_comparison_exp](#gender_enum_enum_comparison_exp)
    * [gender_enum_insert_input](#gender_enum_insert_input)
    * [gender_enum_obj_rel_insert_input](#gender_enum_obj_rel_insert_input)
    * [gender_enum_on_conflict](#gender_enum_on_conflict)
    * [gender_enum_order_by](#gender_enum_order_by)
    * [gender_enum_pk_columns_input](#gender_enum_pk_columns_input)
    * [gender_enum_set_input](#gender_enum_set_input)
    * [patients_aggregate_order_by](#patients_aggregate_order_by)
    * [patients_arr_rel_insert_input](#patients_arr_rel_insert_input)
    * [patients_bool_exp](#patients_bool_exp)
    * [patients_insert_input](#patients_insert_input)
    * [patients_max_order_by](#patients_max_order_by)
    * [patients_min_order_by](#patients_min_order_by)
    * [patients_obj_rel_insert_input](#patients_obj_rel_insert_input)
    * [patients_on_conflict](#patients_on_conflict)
    * [patients_order_by](#patients_order_by)
    * [patients_pk_columns_input](#patients_pk_columns_input)
    * [patients_set_input](#patients_set_input)
    * [prescription_item_aggregate_order_by](#prescription_item_aggregate_order_by)
    * [prescription_item_arr_rel_insert_input](#prescription_item_arr_rel_insert_input)
    * [prescription_item_avg_order_by](#prescription_item_avg_order_by)
    * [prescription_item_bool_exp](#prescription_item_bool_exp)
    * [prescription_item_inc_input](#prescription_item_inc_input)
    * [prescription_item_insert_input](#prescription_item_insert_input)
    * [prescription_item_max_order_by](#prescription_item_max_order_by)
    * [prescription_item_min_order_by](#prescription_item_min_order_by)
    * [prescription_item_on_conflict](#prescription_item_on_conflict)
    * [prescription_item_order_by](#prescription_item_order_by)
    * [prescription_item_pk_columns_input](#prescription_item_pk_columns_input)
    * [prescription_item_set_input](#prescription_item_set_input)
    * [prescription_item_stddev_order_by](#prescription_item_stddev_order_by)
    * [prescription_item_stddev_pop_order_by](#prescription_item_stddev_pop_order_by)
    * [prescription_item_stddev_samp_order_by](#prescription_item_stddev_samp_order_by)
    * [prescription_item_sum_order_by](#prescription_item_sum_order_by)
    * [prescription_item_type_enum_bool_exp](#prescription_item_type_enum_bool_exp)
    * [prescription_item_type_enum_enum_comparison_exp](#prescription_item_type_enum_enum_comparison_exp)
    * [prescription_item_type_enum_insert_input](#prescription_item_type_enum_insert_input)
    * [prescription_item_type_enum_obj_rel_insert_input](#prescription_item_type_enum_obj_rel_insert_input)
    * [prescription_item_type_enum_on_conflict](#prescription_item_type_enum_on_conflict)
    * [prescription_item_type_enum_order_by](#prescription_item_type_enum_order_by)
    * [prescription_item_type_enum_pk_columns_input](#prescription_item_type_enum_pk_columns_input)
    * [prescription_item_type_enum_set_input](#prescription_item_type_enum_set_input)
    * [prescription_item_var_pop_order_by](#prescription_item_var_pop_order_by)
    * [prescription_item_var_samp_order_by](#prescription_item_var_samp_order_by)
    * [prescription_item_variance_order_by](#prescription_item_variance_order_by)
    * [prescriptions_aggregate_order_by](#prescriptions_aggregate_order_by)
    * [prescriptions_arr_rel_insert_input](#prescriptions_arr_rel_insert_input)
    * [prescriptions_bool_exp](#prescriptions_bool_exp)
    * [prescriptions_insert_input](#prescriptions_insert_input)
    * [prescriptions_max_order_by](#prescriptions_max_order_by)
    * [prescriptions_min_order_by](#prescriptions_min_order_by)
    * [prescriptions_obj_rel_insert_input](#prescriptions_obj_rel_insert_input)
    * [prescriptions_on_conflict](#prescriptions_on_conflict)
    * [prescriptions_order_by](#prescriptions_order_by)
    * [prescriptions_pk_columns_input](#prescriptions_pk_columns_input)
    * [prescriptions_set_input](#prescriptions_set_input)
    * [timestamptz_comparison_exp](#timestamptz_comparison_exp)
    * [uuid_comparison_exp](#uuid_comparison_exp)
  * [Enums](#enums)
    * [drugs_constraint](#drugs_constraint)
    * [drugs_select_column](#drugs_select_column)
    * [drugs_update_column](#drugs_update_column)
    * [gender_enum_constraint](#gender_enum_constraint)
    * [gender_enum_enum](#gender_enum_enum)
    * [gender_enum_select_column](#gender_enum_select_column)
    * [gender_enum_update_column](#gender_enum_update_column)
    * [order_by](#order_by)
    * [patients_constraint](#patients_constraint)
    * [patients_select_column](#patients_select_column)
    * [patients_update_column](#patients_update_column)
    * [prescription_item_constraint](#prescription_item_constraint)
    * [prescription_item_select_column](#prescription_item_select_column)
    * [prescription_item_type_enum_constraint](#prescription_item_type_enum_constraint)
    * [prescription_item_type_enum_enum](#prescription_item_type_enum_enum)
    * [prescription_item_type_enum_select_column](#prescription_item_type_enum_select_column)
    * [prescription_item_type_enum_update_column](#prescription_item_type_enum_update_column)
    * [prescription_item_update_column](#prescription_item_update_column)
    * [prescriptions_constraint](#prescriptions_constraint)
    * [prescriptions_select_column](#prescriptions_select_column)
    * [prescriptions_update_column](#prescriptions_update_column)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [Float](#float)
    * [Int](#int)
    * [String](#string)
    * [timestamptz](#timestamptz)
    * [uuid](#uuid)

</details>

## Query (query_root)
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>drugs</strong></td>
<td valign="top">[<a href="#drugs">drugs</a>!]!</td>
<td>

fetch data from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#drugs_select_column">drugs_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#drugs_order_by">drugs_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drugs_aggregate</strong></td>
<td valign="top"><a href="#drugs_aggregate">drugs_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#drugs_select_column">drugs_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#drugs_order_by">drugs_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drugs_by_pk</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

fetch data from the table: "drugs" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top">[<a href="#gender_enum">gender_enum</a>!]!</td>
<td>

fetch data from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#gender_enum_select_column">gender_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#gender_enum_order_by">gender_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum_aggregate</strong></td>
<td valign="top"><a href="#gender_enum_aggregate">gender_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#gender_enum_select_column">gender_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#gender_enum_order_by">gender_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum_by_pk</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a></td>
<td>

fetch data from the table: "gender_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">gender</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients</strong></td>
<td valign="top">[<a href="#patients">patients</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_aggregate</strong></td>
<td valign="top"><a href="#patients_aggregate">patients_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_by_pk</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

fetch data from the table: "patients" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

fetch data from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate">prescription_item_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_by_pk</strong></td>
<td valign="top"><a href="#prescription_item">prescription_item</a></td>
<td>

fetch data from the table: "prescription_item" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum">prescription_item_type_enum</a>!]!</td>
<td>

fetch data from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_type_enum_select_column">prescription_item_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_type_enum_order_by">prescription_item_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_aggregate">prescription_item_type_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_type_enum_select_column">prescription_item_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_type_enum_order_by">prescription_item_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum_by_pk</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

fetch data from the table: "prescription_item_type_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions</strong></td>
<td valign="top">[<a href="#prescriptions">prescriptions</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_aggregate</strong></td>
<td valign="top"><a href="#prescriptions_aggregate">prescriptions_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_by_pk</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

fetch data from the table: "prescriptions" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
</tbody>
</table>

## Mutation (mutation_root)
mutation root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>delete_drugs</strong></td>
<td valign="top"><a href="#drugs_mutation_response">drugs_mutation_response</a></td>
<td>

delete data from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_drugs_by_pk</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

delete single row from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_mutation_response">gender_enum_mutation_response</a></td>
<td>

delete data from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_gender_enum_by_pk</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a></td>
<td>

delete single row from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">gender</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_patients</strong></td>
<td valign="top"><a href="#patients_mutation_response">patients_mutation_response</a></td>
<td>

delete data from the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_patients_by_pk</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

delete single row from the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescription_item</strong></td>
<td valign="top"><a href="#prescription_item_mutation_response">prescription_item_mutation_response</a></td>
<td>

delete data from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescription_item_by_pk</strong></td>
<td valign="top"><a href="#prescription_item">prescription_item</a></td>
<td>

delete single row from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_mutation_response">prescription_item_type_enum_mutation_response</a></td>
<td>

delete data from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescription_item_type_enum_by_pk</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

delete single row from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescriptions</strong></td>
<td valign="top"><a href="#prescriptions_mutation_response">prescriptions_mutation_response</a></td>
<td>

delete data from the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_prescriptions_by_pk</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

delete single row from the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_drugs</strong></td>
<td valign="top"><a href="#drugs_mutation_response">drugs_mutation_response</a></td>
<td>

insert data into the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#drugs_insert_input">drugs_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#drugs_on_conflict">drugs_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_drugs_one</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

insert a single row into the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#drugs_insert_input">drugs_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#drugs_on_conflict">drugs_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_mutation_response">gender_enum_mutation_response</a></td>
<td>

insert data into the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#gender_enum_insert_input">gender_enum_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#gender_enum_on_conflict">gender_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_gender_enum_one</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a></td>
<td>

insert a single row into the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#gender_enum_insert_input">gender_enum_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#gender_enum_on_conflict">gender_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_patients</strong></td>
<td valign="top"><a href="#patients_mutation_response">patients_mutation_response</a></td>
<td>

insert data into the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#patients_insert_input">patients_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#patients_on_conflict">patients_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_patients_one</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

insert a single row into the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#patients_insert_input">patients_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#patients_on_conflict">patients_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescription_item</strong></td>
<td valign="top"><a href="#prescription_item_mutation_response">prescription_item_mutation_response</a></td>
<td>

insert data into the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#prescription_item_insert_input">prescription_item_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescription_item_on_conflict">prescription_item_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescription_item_one</strong></td>
<td valign="top"><a href="#prescription_item">prescription_item</a></td>
<td>

insert a single row into the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#prescription_item_insert_input">prescription_item_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescription_item_on_conflict">prescription_item_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_mutation_response">prescription_item_type_enum_mutation_response</a></td>
<td>

insert data into the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#prescription_item_type_enum_insert_input">prescription_item_type_enum_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescription_item_type_enum_on_conflict">prescription_item_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescription_item_type_enum_one</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

insert a single row into the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#prescription_item_type_enum_insert_input">prescription_item_type_enum_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescription_item_type_enum_on_conflict">prescription_item_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescriptions</strong></td>
<td valign="top"><a href="#prescriptions_mutation_response">prescriptions_mutation_response</a></td>
<td>

insert data into the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#prescriptions_insert_input">prescriptions_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescriptions_on_conflict">prescriptions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_prescriptions_one</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

insert a single row into the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#prescriptions_insert_input">prescriptions_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#prescriptions_on_conflict">prescriptions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_drugs</strong></td>
<td valign="top"><a href="#drugs_mutation_response">drugs_mutation_response</a></td>
<td>

update data of the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#drugs_set_input">drugs_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_drugs_by_pk</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

update single row of the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#drugs_set_input">drugs_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#drugs_pk_columns_input">drugs_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_mutation_response">gender_enum_mutation_response</a></td>
<td>

update data of the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#gender_enum_set_input">gender_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_gender_enum_by_pk</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a></td>
<td>

update single row of the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#gender_enum_set_input">gender_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#gender_enum_pk_columns_input">gender_enum_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_patients</strong></td>
<td valign="top"><a href="#patients_mutation_response">patients_mutation_response</a></td>
<td>

update data of the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#patients_set_input">patients_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_patients_by_pk</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

update single row of the table: "patients"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#patients_set_input">patients_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#patients_pk_columns_input">patients_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescription_item</strong></td>
<td valign="top"><a href="#prescription_item_mutation_response">prescription_item_mutation_response</a></td>
<td>

update data of the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#prescription_item_inc_input">prescription_item_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescription_item_set_input">prescription_item_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescription_item_by_pk</strong></td>
<td valign="top"><a href="#prescription_item">prescription_item</a></td>
<td>

update single row of the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#prescription_item_inc_input">prescription_item_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescription_item_set_input">prescription_item_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#prescription_item_pk_columns_input">prescription_item_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_mutation_response">prescription_item_type_enum_mutation_response</a></td>
<td>

update data of the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescription_item_type_enum_set_input">prescription_item_type_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescription_item_type_enum_by_pk</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

update single row of the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescription_item_type_enum_set_input">prescription_item_type_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#prescription_item_type_enum_pk_columns_input">prescription_item_type_enum_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescriptions</strong></td>
<td valign="top"><a href="#prescriptions_mutation_response">prescriptions_mutation_response</a></td>
<td>

update data of the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescriptions_set_input">prescriptions_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_prescriptions_by_pk</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

update single row of the table: "prescriptions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#prescriptions_set_input">prescriptions_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#prescriptions_pk_columns_input">prescriptions_pk_columns_input</a>!</td>
<td></td>
</tr>
</tbody>
</table>

## Objects

### drugs

columns and relationships of "drugs"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td>

When it was imported to this system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_controlled_drug</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

The drug name as it's found in dm+d

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate">prescription_item_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td>

When it was last updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_aggregate

aggregated selection of "drugs"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#drugs_aggregate_fields">drugs_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#drugs">drugs</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### drugs_aggregate_fields

aggregate fields of "drugs"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#drugs_select_column">drugs_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#drugs_max_fields">drugs_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#drugs_min_fields">drugs_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was imported to this system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The drug name as it's found in dm+d

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was last updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was imported to this system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The drug name as it's found in dm+d

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was last updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_mutation_response

response of any mutation on the table "drugs"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#drugs">drugs</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### gender_enum

columns and relationships of "gender_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients</strong></td>
<td valign="top">[<a href="#patients">patients</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_aggregate</strong></td>
<td valign="top"><a href="#patients_aggregate">patients_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

### gender_enum_aggregate

aggregated selection of "gender_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#gender_enum_aggregate_fields">gender_enum_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#gender_enum">gender_enum</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_aggregate_fields

aggregate fields of "gender_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#gender_enum_select_column">gender_enum_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#gender_enum_max_fields">gender_enum_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#gender_enum_min_fields">gender_enum_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_mutation_response

response of any mutation on the table "gender_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#gender_enum">gender_enum</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### patients

columns and relationships of "patients"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#gender_enum_enum">gender_enum_enum</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions</strong></td>
<td valign="top">[<a href="#prescriptions">prescriptions</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_aggregate</strong></td>
<td valign="top"><a href="#prescriptions_aggregate">prescriptions_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_aggregate

aggregated selection of "patients"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#patients_aggregate_fields">patients_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#patients">patients</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### patients_aggregate_fields

aggregate fields of "patients"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#patients_max_fields">patients_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#patients_min_fields">patients_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_mutation_response

response of any mutation on the table "patients"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#patients">patients</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### prescription_item

columns and relationships of "prescription_item"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_schedule</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_prn</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_aggregate

aggregated selection of "prescription_item"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate_fields">prescription_item_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_aggregate_fields

aggregate fields of "prescription_item"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#prescription_item_avg_fields">prescription_item_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#prescription_item_max_fields">prescription_item_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#prescription_item_min_fields">prescription_item_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#prescription_item_stddev_fields">prescription_item_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#prescription_item_stddev_pop_fields">prescription_item_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#prescription_item_stddev_samp_fields">prescription_item_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#prescription_item_sum_fields">prescription_item_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#prescription_item_var_pop_fields">prescription_item_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#prescription_item_var_samp_fields">prescription_item_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#prescription_item_variance_fields">prescription_item_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_mutation_response

response of any mutation on the table "prescription_item"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### prescription_item_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum

columns and relationships of "prescription_item_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate">prescription_item_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_aggregate

aggregated selection of "prescription_item_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_aggregate_fields">prescription_item_type_enum_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum">prescription_item_type_enum</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_aggregate_fields

aggregate fields of "prescription_item_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#prescription_item_type_enum_select_column">prescription_item_type_enum_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_max_fields">prescription_item_type_enum_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_min_fields">prescription_item_type_enum_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_mutation_response

response of any mutation on the table "prescription_item_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum">prescription_item_type_enum</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### prescription_item_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions

columns and relationships of "prescriptions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate">prescription_item_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_aggregate

aggregated selection of "prescriptions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#prescriptions_aggregate_fields">prescriptions_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#prescriptions">prescriptions</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_aggregate_fields

aggregate fields of "prescriptions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#prescriptions_max_fields">prescriptions_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#prescriptions_min_fields">prescriptions_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_mutation_response

response of any mutation on the table "prescriptions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#prescriptions">prescriptions</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### subscription_root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>drugs</strong></td>
<td valign="top">[<a href="#drugs">drugs</a>!]!</td>
<td>

fetch data from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#drugs_select_column">drugs_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#drugs_order_by">drugs_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drugs_aggregate</strong></td>
<td valign="top"><a href="#drugs_aggregate">drugs_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "drugs"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#drugs_select_column">drugs_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#drugs_order_by">drugs_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drugs_by_pk</strong></td>
<td valign="top"><a href="#drugs">drugs</a></td>
<td>

fetch data from the table: "drugs" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top">[<a href="#gender_enum">gender_enum</a>!]!</td>
<td>

fetch data from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#gender_enum_select_column">gender_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#gender_enum_order_by">gender_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum_aggregate</strong></td>
<td valign="top"><a href="#gender_enum_aggregate">gender_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "gender_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#gender_enum_select_column">gender_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#gender_enum_order_by">gender_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum_by_pk</strong></td>
<td valign="top"><a href="#gender_enum">gender_enum</a></td>
<td>

fetch data from the table: "gender_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">gender</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients</strong></td>
<td valign="top">[<a href="#patients">patients</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_aggregate</strong></td>
<td valign="top"><a href="#patients_aggregate">patients_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patients_select_column">patients_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#patients_order_by">patients_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_by_pk</strong></td>
<td valign="top"><a href="#patients">patients</a></td>
<td>

fetch data from the table: "patients" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item</strong></td>
<td valign="top">[<a href="#prescription_item">prescription_item</a>!]!</td>
<td>

fetch data from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate">prescription_item_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "prescription_item"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_select_column">prescription_item_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_order_by">prescription_item_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_by_pk</strong></td>
<td valign="top"><a href="#prescription_item">prescription_item</a></td>
<td>

fetch data from the table: "prescription_item" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum">prescription_item_type_enum</a>!]!</td>
<td>

fetch data from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_type_enum_select_column">prescription_item_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_type_enum_order_by">prescription_item_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_aggregate">prescription_item_type_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "prescription_item_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescription_item_type_enum_select_column">prescription_item_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescription_item_type_enum_order_by">prescription_item_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum_by_pk</strong></td>
<td valign="top"><a href="#prescription_item_type_enum">prescription_item_type_enum</a></td>
<td>

fetch data from the table: "prescription_item_type_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">type</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions</strong></td>
<td valign="top">[<a href="#prescriptions">prescriptions</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_aggregate</strong></td>
<td valign="top"><a href="#prescriptions_aggregate">prescriptions_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#prescriptions_select_column">prescriptions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#prescriptions_order_by">prescriptions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_by_pk</strong></td>
<td valign="top"><a href="#prescriptions">prescriptions</a></td>
<td>

fetch data from the table: "prescriptions" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
</tbody>
</table>

## Inputs

### Boolean_comparison_exp

Boolean expression to compare columns of type "Boolean". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#boolean">Boolean</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#boolean">Boolean</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### Int_comparison_exp

Boolean expression to compare columns of type "Int". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### String_comparison_exp

Boolean expression to compare columns of type "String". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_ilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given case-insensitive pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_iregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given POSIX regular expression, case insensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_like</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given case-insensitive pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_niregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given POSIX regular expression, case insensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nlike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given POSIX regular expression, case sensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nsimilar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given SQL regular expression

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_regex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given POSIX regular expression, case sensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_similar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given SQL regular expression

</td>
</tr>
</tbody>
</table>

### drugs_bool_exp

Boolean expression to filter rows from the table "drugs". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#drugs_bool_exp">drugs_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#drugs_bool_exp">drugs_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_controlled_drug</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_insert_input

input type for inserting data into table "drugs"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was imported to this system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_controlled_drug</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The drug name as it's found in dm+d

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_arr_rel_insert_input">prescription_item_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was last updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_obj_rel_insert_input

input type for inserting object relation for remote table "drugs"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#drugs_insert_input">drugs_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#drugs_on_conflict">drugs_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### drugs_on_conflict

on conflict condition type for table "drugs"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#drugs_constraint">drugs_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#drugs_update_column">drugs_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_order_by

Ordering options when selecting data from "drugs".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_controlled_drug</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate_order_by">prescription_item_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### drugs_pk_columns_input

primary key columns input for table: drugs

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td>

Internal CHS ID

</td>
</tr>
</tbody>
</table>

### drugs_set_input

input type for updating data in table "drugs"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was imported to this system

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dmd_code</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td>

Internal CHS ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>image</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_controlled_drug</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The drug name as it's found in dm+d

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td>

When it was last updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_bool_exp

Boolean expression to filter rows from the table "gender_enum". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#gender_enum_bool_exp">gender_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#gender_enum_bool_exp">gender_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients</strong></td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_enum_comparison_exp

Boolean expression to compare columns of type "gender_enum_enum". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#gender_enum_enum">gender_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#gender_enum_enum">gender_enum_enum</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#gender_enum_enum">gender_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#gender_enum_enum">gender_enum_enum</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_insert_input

input type for inserting data into table "gender_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients</strong></td>
<td valign="top"><a href="#patients_arr_rel_insert_input">patients_arr_rel_insert_input</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_obj_rel_insert_input

input type for inserting object relation for remote table "gender_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#gender_enum_insert_input">gender_enum_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#gender_enum_on_conflict">gender_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### gender_enum_on_conflict

on conflict condition type for table "gender_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#gender_enum_constraint">gender_enum_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#gender_enum_update_column">gender_enum_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_order_by

Ordering options when selecting data from "gender_enum".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patients_aggregate</strong></td>
<td valign="top"><a href="#patients_aggregate_order_by">patients_aggregate_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_pk_columns_input

primary key columns input for table: gender_enum

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_set_input

input type for updating data in table "gender_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_aggregate_order_by

order by aggregate values of table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#patients_max_order_by">patients_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#patients_min_order_by">patients_min_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_arr_rel_insert_input

input type for inserting array relation for remote table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#patients_insert_input">patients_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#patients_on_conflict">patients_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### patients_bool_exp

Boolean expression to filter rows from the table "patients". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#patients_bool_exp">patients_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#patients_bool_exp">patients_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#gender_enum_enum_comparison_exp">gender_enum_enum_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_bool_exp">gender_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions</strong></td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_insert_input

input type for inserting data into table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#gender_enum_enum">gender_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_obj_rel_insert_input">gender_enum_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions</strong></td>
<td valign="top"><a href="#prescriptions_arr_rel_insert_input">prescriptions_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_max_order_by

order by max() on columns of table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_min_order_by

order by min() on columns of table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_obj_rel_insert_input

input type for inserting object relation for remote table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#patients_insert_input">patients_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#patients_on_conflict">patients_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### patients_on_conflict

on conflict condition type for table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#patients_constraint">patients_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#patients_update_column">patients_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_order_by

Ordering options when selecting data from "patients".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender_enum</strong></td>
<td valign="top"><a href="#gender_enum_order_by">gender_enum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriptions_aggregate</strong></td>
<td valign="top"><a href="#prescriptions_aggregate_order_by">prescriptions_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patients_pk_columns_input

primary key columns input for table: patients

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### patients_set_input

input type for updating data in table "patients"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>address_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_2</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_3</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_4</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>address_5</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>city</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>country</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>county</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>date_of_birth</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>first_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>gender</strong></td>
<td valign="top"><a href="#gender_enum_enum">gender_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>mobile_phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nhs_number</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phone_1</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>postcode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>surname</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_aggregate_order_by

order by aggregate values of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#prescription_item_avg_order_by">prescription_item_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#prescription_item_max_order_by">prescription_item_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#prescription_item_min_order_by">prescription_item_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#prescription_item_stddev_order_by">prescription_item_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#prescription_item_stddev_pop_order_by">prescription_item_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#prescription_item_stddev_samp_order_by">prescription_item_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#prescription_item_sum_order_by">prescription_item_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#prescription_item_var_pop_order_by">prescription_item_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#prescription_item_var_samp_order_by">prescription_item_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#prescription_item_variance_order_by">prescription_item_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_arr_rel_insert_input

input type for inserting array relation for remote table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#prescription_item_insert_input">prescription_item_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#prescription_item_on_conflict">prescription_item_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### prescription_item_avg_order_by

order by avg() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_bool_exp

Boolean expression to filter rows from the table "prescription_item". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#prescription_item_bool_exp">prescription_item_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#prescription_item_bool_exp">prescription_item_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug</strong></td>
<td valign="top"><a href="#drugs_bool_exp">drugs_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_schedule</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_prn</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription</strong></td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum_comparison_exp">prescription_item_type_enum_enum_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_inc_input

input type for incrementing numeric columns in table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_insert_input

input type for inserting data into table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug</strong></td>
<td valign="top"><a href="#drugs_obj_rel_insert_input">drugs_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_schedule</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_prn</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription</strong></td>
<td valign="top"><a href="#prescriptions_obj_rel_insert_input">prescriptions_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_obj_rel_insert_input">prescription_item_type_enum_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_max_order_by

order by max() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_min_order_by

order by min() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_on_conflict

on conflict condition type for table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#prescription_item_constraint">prescription_item_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#prescription_item_update_column">prescription_item_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_order_by

Ordering options when selecting data from "prescription_item".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug</strong></td>
<td valign="top"><a href="#drugs_order_by">drugs_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_schedule</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_prn</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription</strong></td>
<td valign="top"><a href="#prescriptions_order_by">prescriptions_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_item_type_enum</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_order_by">prescription_item_type_enum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_pk_columns_input

primary key columns input for table: prescription_item

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_set_input

input type for updating data in table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delivered_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dosage_instructions</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>drug_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_schedule</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_prn</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_received_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shipped_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_stddev_order_by

order by stddev() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_stddev_pop_order_by

order by stddev_pop() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_stddev_samp_order_by

order by stddev_samp() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_sum_order_by

order by sum() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_bool_exp

Boolean expression to filter rows from the table "prescription_item_type_enum". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_enum_comparison_exp

Boolean expression to compare columns of type "prescription_item_type_enum_enum". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum_enum">prescription_item_type_enum_enum</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_insert_input

input type for inserting data into table "prescription_item_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_arr_rel_insert_input">prescription_item_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_obj_rel_insert_input

input type for inserting object relation for remote table "prescription_item_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_insert_input">prescription_item_type_enum_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_on_conflict">prescription_item_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_on_conflict

on conflict condition type for table "prescription_item_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_constraint">prescription_item_type_enum_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#prescription_item_type_enum_update_column">prescription_item_type_enum_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#prescription_item_type_enum_bool_exp">prescription_item_type_enum_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_order_by

Ordering options when selecting data from "prescription_item_type_enum".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate_order_by">prescription_item_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_pk_columns_input

primary key columns input for table: prescription_item_type_enum

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_set_input

input type for updating data in table "prescription_item_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_var_pop_order_by

order by var_pop() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_var_samp_order_by

order by var_samp() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_variance_order_by

order by variance() on columns of table "prescription_item"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>quantity_prescribed</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>quantity_supplied</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_aggregate_order_by

order by aggregate values of table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#prescriptions_max_order_by">prescriptions_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#prescriptions_min_order_by">prescriptions_min_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_arr_rel_insert_input

input type for inserting array relation for remote table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#prescriptions_insert_input">prescriptions_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#prescriptions_on_conflict">prescriptions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### prescriptions_bool_exp

Boolean expression to filter rows from the table "prescriptions". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#prescriptions_bool_exp">prescriptions_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#prescriptions_bool_exp">prescriptions_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient</strong></td>
<td valign="top"><a href="#patients_bool_exp">patients_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid_comparison_exp">uuid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_bool_exp">prescription_item_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_insert_input

input type for inserting data into table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient</strong></td>
<td valign="top"><a href="#patients_obj_rel_insert_input">patients_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items</strong></td>
<td valign="top"><a href="#prescription_item_arr_rel_insert_input">prescription_item_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_max_order_by

order by max() on columns of table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_min_order_by

order by min() on columns of table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_obj_rel_insert_input

input type for inserting object relation for remote table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#prescriptions_insert_input">prescriptions_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#prescriptions_on_conflict">prescriptions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### prescriptions_on_conflict

on conflict condition type for table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#prescriptions_constraint">prescriptions_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#prescriptions_update_column">prescriptions_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#prescriptions_bool_exp">prescriptions_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_order_by

Ordering options when selecting data from "prescriptions".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient</strong></td>
<td valign="top"><a href="#patients_order_by">patients_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescription_items_aggregate</strong></td>
<td valign="top"><a href="#prescription_item_aggregate_order_by">prescription_item_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_pk_columns_input

primary key columns input for table: prescriptions

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### prescriptions_set_input

input type for updating data in table "prescriptions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescribed_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prescriber</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### timestamptz_comparison_exp

Boolean expression to compare columns of type "timestamptz". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### uuid_comparison_exp

Boolean expression to compare columns of type "uuid". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#uuid">uuid</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#uuid">uuid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#uuid">uuid</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

## Enums

### drugs_constraint

unique or primary key constraints on table "drugs"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>dmd_code_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>dmd_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### drugs_select_column

select columns of table "drugs"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dmd_code</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>image</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>is_controlled_drug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>warnings</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### drugs_update_column

update columns of table "drugs"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dmd_code</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>image</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>is_controlled_drug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>warnings</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### gender_enum_constraint

unique or primary key constraints on table "gender_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>gender_enum_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### gender_enum_enum

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>female</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>male</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>nb</strong></td>
<td></td>
</tr>
</tbody>
</table>

### gender_enum_select_column

select columns of table "gender_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>gender</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### gender_enum_update_column

update columns of table "gender_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>gender</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### order_by

column ordering options

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>asc</strong></td>
<td>

in ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_first</strong></td>
<td>

in ascending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_last</strong></td>
<td>

in ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>desc</strong></td>
<td>

in descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_first</strong></td>
<td>

in descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_last</strong></td>
<td>

in descending order, nulls last

</td>
</tr>
</tbody>
</table>

### patients_constraint

unique or primary key constraints on table "patients"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>patients_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### patients_select_column

select columns of table "patients"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>address_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_2</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_3</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_4</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_5</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>city</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>country</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>county</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>date_of_birth</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>first_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>gender</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>mobile_phone_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>nhs_number</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>phone_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>postcode</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>surname</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### patients_update_column

update columns of table "patients"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>address_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_2</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_3</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_4</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>address_5</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>city</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>country</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>county</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>date_of_birth</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>first_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>gender</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>mobile_phone_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>nhs_number</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>phone_1</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>postcode</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>surname</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescription_item_constraint

unique or primary key constraints on table "prescription_item"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>medications_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### prescription_item_select_column

select columns of table "prescription_item"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>delivered_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dispensed_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dosage_instructions</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>drug_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>has_schedule</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>is_prn</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescription_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescription_received_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>quantity_prescribed</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>quantity_supplied</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>shipped_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_constraint

unique or primary key constraints on table "prescription_item_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>dmd_type_enum_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_enum

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>Acute</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Repeat</strong></td>
<td></td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_select_column

select columns of table "prescription_item_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>type</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescription_item_type_enum_update_column

update columns of table "prescription_item_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>type</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescription_item_update_column

update columns of table "prescription_item"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>delivered_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dispensed_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dosage_instructions</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>drug_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>has_schedule</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>is_prn</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescription_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescription_received_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>quantity_prescribed</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>quantity_supplied</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>shipped_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescriptions_constraint

unique or primary key constraints on table "prescriptions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>prescription_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### prescriptions_select_column

select columns of table "prescriptions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>patient_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescribed_date</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescriber</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### prescriptions_update_column

update columns of table "prescriptions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>patient_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescribed_date</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prescriber</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

### Float

### Int

### String

### timestamptz

### uuid

