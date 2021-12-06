# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Objects](#objects)
    * [drugs](#drugs)
    * [gender_enum](#gender_enum)
    * [organisations](#organisations)
    * [patient_consent](#patient_consent)
    * [patients](#patients)
    * [prescription_item](#prescription_item)
    * [prescription_item_type_enum](#prescription_item_type_enum)
    * [prescriptions](#prescriptions)
    * [subscription_root](#subscription_root)
  * [Inputs](#inputs)
    * [Boolean_comparison_exp](#boolean_comparison_exp)
    * [Int_comparison_exp](#int_comparison_exp)
    * [String_comparison_exp](#string_comparison_exp)
    * [drugs_bool_exp](#drugs_bool_exp)
    * [drugs_order_by](#drugs_order_by)
    * [gender_enum_bool_exp](#gender_enum_bool_exp)
    * [gender_enum_enum_comparison_exp](#gender_enum_enum_comparison_exp)
    * [gender_enum_order_by](#gender_enum_order_by)
    * [organisations_bool_exp](#organisations_bool_exp)
    * [organisations_order_by](#organisations_order_by)
    * [patient_consent_aggregate_order_by](#patient_consent_aggregate_order_by)
    * [patient_consent_bool_exp](#patient_consent_bool_exp)
    * [patient_consent_max_order_by](#patient_consent_max_order_by)
    * [patient_consent_min_order_by](#patient_consent_min_order_by)
    * [patient_consent_order_by](#patient_consent_order_by)
    * [patients_aggregate_order_by](#patients_aggregate_order_by)
    * [patients_bool_exp](#patients_bool_exp)
    * [patients_max_order_by](#patients_max_order_by)
    * [patients_min_order_by](#patients_min_order_by)
    * [patients_order_by](#patients_order_by)
    * [prescription_item_aggregate_order_by](#prescription_item_aggregate_order_by)
    * [prescription_item_avg_order_by](#prescription_item_avg_order_by)
    * [prescription_item_bool_exp](#prescription_item_bool_exp)
    * [prescription_item_max_order_by](#prescription_item_max_order_by)
    * [prescription_item_min_order_by](#prescription_item_min_order_by)
    * [prescription_item_order_by](#prescription_item_order_by)
    * [prescription_item_stddev_order_by](#prescription_item_stddev_order_by)
    * [prescription_item_stddev_pop_order_by](#prescription_item_stddev_pop_order_by)
    * [prescription_item_stddev_samp_order_by](#prescription_item_stddev_samp_order_by)
    * [prescription_item_sum_order_by](#prescription_item_sum_order_by)
    * [prescription_item_type_enum_bool_exp](#prescription_item_type_enum_bool_exp)
    * [prescription_item_type_enum_enum_comparison_exp](#prescription_item_type_enum_enum_comparison_exp)
    * [prescription_item_type_enum_order_by](#prescription_item_type_enum_order_by)
    * [prescription_item_var_pop_order_by](#prescription_item_var_pop_order_by)
    * [prescription_item_var_samp_order_by](#prescription_item_var_samp_order_by)
    * [prescription_item_variance_order_by](#prescription_item_variance_order_by)
    * [prescriptions_aggregate_order_by](#prescriptions_aggregate_order_by)
    * [prescriptions_bool_exp](#prescriptions_bool_exp)
    * [prescriptions_max_order_by](#prescriptions_max_order_by)
    * [prescriptions_min_order_by](#prescriptions_min_order_by)
    * [prescriptions_order_by](#prescriptions_order_by)
    * [timestamptz_comparison_exp](#timestamptz_comparison_exp)
    * [uuid_comparison_exp](#uuid_comparison_exp)
  * [Enums](#enums)
    * [drugs_select_column](#drugs_select_column)
    * [gender_enum_enum](#gender_enum_enum)
    * [gender_enum_select_column](#gender_enum_select_column)
    * [order_by](#order_by)
    * [organisations_select_column](#organisations_select_column)
    * [patient_consent_select_column](#patient_consent_select_column)
    * [patients_select_column](#patients_select_column)
    * [prescription_item_select_column](#prescription_item_select_column)
    * [prescription_item_type_enum_enum](#prescription_item_type_enum_enum)
    * [prescription_item_type_enum_select_column](#prescription_item_type_enum_select_column)
    * [prescriptions_select_column](#prescriptions_select_column)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
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
<td colspan="2" valign="top"><strong>organisations</strong></td>
<td valign="top">[<a href="#organisations">organisations</a>!]!</td>
<td>

fetch data from the table: "organisations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#organisations_select_column">organisations_select_column</a>!]</td>
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
<td valign="top">[<a href="#organisations_order_by">organisations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#organisations_bool_exp">organisations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organisations_by_pk</strong></td>
<td valign="top"><a href="#organisations">organisations</a></td>
<td>

fetch data from the table: "organisations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consent</strong></td>
<td valign="top">[<a href="#patient_consent">patient_consent</a>!]!</td>
<td>

fetch data from the table: "patient_consent"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patient_consent_select_column">patient_consent_select_column</a>!]</td>
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
<td valign="top">[<a href="#patient_consent_order_by">patient_consent_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consent_by_pk</strong></td>
<td valign="top"><a href="#patient_consent">patient_consent</a></td>
<td>

fetch data from the table: "patient_consent" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
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
</tbody>
</table>

### organisations

columns and relationships of "organisations"

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
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consents</strong></td>
<td valign="top">[<a href="#patient_consent">patient_consent</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patient_consent_select_column">patient_consent_select_column</a>!]</td>
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
<td valign="top">[<a href="#patient_consent_order_by">patient_consent_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
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

### patient_consent

columns and relationships of "patient_consent"

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
<td colspan="2" valign="top"><strong>organisation</strong></td>
<td valign="top"><a href="#organisations">organisations</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organisation_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient</strong></td>
<td valign="top"><a href="#patients">patients</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
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
<td colspan="2" valign="top"><strong>patient_consents</strong></td>
<td valign="top">[<a href="#patient_consent">patient_consent</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patient_consent_select_column">patient_consent_select_column</a>!]</td>
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
<td valign="top">[<a href="#patient_consent_order_by">patient_consent_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
<td>

filter the rows returned

</td>
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
<td colspan="2" valign="top"><strong>delivered_date</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_date</strong></td>
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
<td colspan="2" valign="top"><strong>prescription_received_date</strong></td>
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
<td colspan="2" valign="top"><strong>shipped_date</strong></td>
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
<td colspan="2" valign="top"><strong>type</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
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
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
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
<td colspan="2" valign="top"><strong>organisations</strong></td>
<td valign="top">[<a href="#organisations">organisations</a>!]!</td>
<td>

fetch data from the table: "organisations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#organisations_select_column">organisations_select_column</a>!]</td>
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
<td valign="top">[<a href="#organisations_order_by">organisations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#organisations_bool_exp">organisations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organisations_by_pk</strong></td>
<td valign="top"><a href="#organisations">organisations</a></td>
<td>

fetch data from the table: "organisations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consent</strong></td>
<td valign="top">[<a href="#patient_consent">patient_consent</a>!]!</td>
<td>

fetch data from the table: "patient_consent"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#patient_consent_select_column">patient_consent_select_column</a>!]</td>
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
<td valign="top">[<a href="#patient_consent_order_by">patient_consent_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consent_by_pk</strong></td>
<td valign="top"><a href="#patient_consent">patient_consent</a></td>
<td>

fetch data from the table: "patient_consent" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">id</td>
<td valign="top"><a href="#uuid">uuid</a>!</td>
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

### organisations_bool_exp

Boolean expression to filter rows from the table "organisations". All fields are combined with a logical 'AND'.

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
<td valign="top">[<a href="#organisations_bool_exp">organisations_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#organisations_bool_exp">organisations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#organisations_bool_exp">organisations_bool_exp</a>!]</td>
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
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consents</strong></td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### organisations_order_by

Ordering options when selecting data from "organisations".

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
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_consents_aggregate</strong></td>
<td valign="top"><a href="#patient_consent_aggregate_order_by">patient_consent_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patient_consent_aggregate_order_by

order by aggregate values of table "patient_consent"

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
<td valign="top"><a href="#patient_consent_max_order_by">patient_consent_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#patient_consent_min_order_by">patient_consent_min_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### patient_consent_bool_exp

Boolean expression to filter rows from the table "patient_consent". All fields are combined with a logical 'AND'.

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
<td valign="top">[<a href="#patient_consent_bool_exp">patient_consent_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#patient_consent_bool_exp">patient_consent_bool_exp</a>!]</td>
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
<td colspan="2" valign="top"><strong>organisation</strong></td>
<td valign="top"><a href="#organisations_bool_exp">organisations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organisation_id</strong></td>
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
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### patient_consent_max_order_by

order by max() on columns of table "patient_consent"

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
<td colspan="2" valign="top"><strong>organisation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
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

### patient_consent_min_order_by

order by min() on columns of table "patient_consent"

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
<td colspan="2" valign="top"><strong>organisation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>patient_id</strong></td>
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

### patient_consent_order_by

Ordering options when selecting data from "patient_consent".

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
<td colspan="2" valign="top"><strong>organisation</strong></td>
<td valign="top"><a href="#organisations_order_by">organisations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>organisation_id</strong></td>
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
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
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
<td colspan="2" valign="top"><strong>patient_consents</strong></td>
<td valign="top"><a href="#patient_consent_bool_exp">patient_consent_bool_exp</a></td>
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
<td colspan="2" valign="top"><strong>patient_consents_aggregate</strong></td>
<td valign="top"><a href="#patient_consent_aggregate_order_by">patient_consent_aggregate_order_by</a></td>
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
<td colspan="2" valign="top"><strong>delivered_date</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_date</strong></td>
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
<td colspan="2" valign="top"><strong>prescription_received_date</strong></td>
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
<td colspan="2" valign="top"><strong>shipped_date</strong></td>
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
<td colspan="2" valign="top"><strong>delivered_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_date</strong></td>
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
<td colspan="2" valign="top"><strong>prescription_received_date</strong></td>
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
<td colspan="2" valign="top"><strong>shipped_date</strong></td>
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
<td colspan="2" valign="top"><strong>delivered_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_date</strong></td>
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
<td colspan="2" valign="top"><strong>prescription_received_date</strong></td>
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
<td colspan="2" valign="top"><strong>shipped_date</strong></td>
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
<td colspan="2" valign="top"><strong>delivered_date</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dispensed_date</strong></td>
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
<td colspan="2" valign="top"><strong>prescription_received_date</strong></td>
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
<td colspan="2" valign="top"><strong>shipped_date</strong></td>
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

### organisations_select_column

select columns of table "organisations"

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
</tbody>
</table>

### patient_consent_select_column

select columns of table "patient_consent"

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
<td valign="top"><strong>organisation_id</strong></td>
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
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

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
<td valign="top"><strong>delivered_date</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>dispensed_date</strong></td>
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
<td valign="top"><strong>prescription_received_date</strong></td>
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
<td valign="top"><strong>shipped_date</strong></td>
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

## Scalars

### Boolean

### Int

### String

### timestamptz

### uuid

