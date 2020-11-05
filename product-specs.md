# Release 1 Specs

## Introduction
We’ve grouped required features into feature sets – and are providing visibility into which features we expect to be built out at the alpha and beta stages. We aim to finish the alpha features in October, setting up the user team to have a functional base product on top of which the beta product can be built ahead of the Q2 2021.


## Overview of Releases
### Alpha Feature Set
* Data Sets - Basic
* Global Data Sets
* Account Management - Basic
* Export
* Access Control - Basic

### Beta Feature Set
* Data Sets - Advanced
* Account Management - Advanced
* Search
* Compare
* API Access
* Access Control - Advanced



## Feature Sets in Detail
### Data Set Management - Basic	
* View index of data sets
    * Index of data sets owned by user
    * Index of data sets owned per specialist
    * Index of favourite data sets 
* Create new data sets
    * Provide metadata about data set
    * Build data template
        * Create basic fields
        * Create field type
        * Set validation rules for global data set field type
            * Ability to pick options for global data set type i.e. restrictions on which options are available for data entry
        * Mark field as required
        * Reorder fields
        * Delete fields
        * Rename fields
    * Publish data template
* Edit existing data template
    * Edit metadata about data set
    * Edit field names
    * Edit field type if no data attached to DS/field
    * Delete field if no data attached to DS/field
* View data set
    * View metadata for data set
    * Owner
    * Name
    * Description
    * Date created
    * View data template fields
    * View data in data set
* Data management
    * Can enter new data into a form 
    * Can view single record in detail
    * Can archive a record from the data set
    * Can restore a record from the data set in 30 days
    * Can filter data in data set
* Archive data set
* Un-archive data set


### 
### Data Set Management - Advanced
*   Create draft of data set (complete later)
*   Field validation
    *   Ability to create a list of options for text type
    *   Ability to create a range of numbers for number type
*   Provide example data for fields
*   Ability to duplicate data sets
*   Ability to make complex fields from global set
    *   **Measures** — amount + global data set of measurements (e.g. volumes) w/ automatic conversion (e.g. 1000ml =  1L)
    *   **Ratios** - amont + ratio of global data set of 2 measures 
    *   **Arrays** - multi-select
    *   **Advanced text** - email address validation, phone number validation, short text, long text
    *   **Location** - the location type of field should work by taking any data submitted and generating a full complement of data above the detail line. More detail below.
*   Can edit existing data
*   Can view edit history
*   Can revert to previous point in edit history
*   Can import a simple spreadsheet (simple means clear column names and data) into existing data set
    *   import type should be csv
    *   data validation should occur before importation and invalid data should not be accessible for analysis until it has been edited
*   advanced filtering


### Global Data Sets
*   Create new global data sets (restricted access)
*   Global DS available as field types (unrestricted access)
*   Users can add fields to global DS (unrestricted access)


### Account Management - Basic
*   Create new account with email
*   Log in to existing account using one-time password


### Account Management - Advanced
*   Suspend accounts
*   Create new account with Ontario.ca
*   View user profile
*   Edit user profile


### Search - Basic
*   Search for a user by name
*   Search for a data set by name
*   Search for a data set by combination of factors – name, keyword, owner, creation date range


### Compare
*   Generate a temporary data set using a search 
    *   Save search parameters
    *   Download generated data set as spreadsheet


### Export
*   Download data as spreadsheet - Download entire data set


### API Access
*   API authorization for external users
*   Retrieve, add, and update data via API endpoints
*   Retrieve data via API endpoint with query parameters in API call


### Access Control - Basic
*   Users and admins only
*   Users have access to their own data sets
*   Users can invite other users to enter data into their own data sets
*   Admins can use an allow list to decide who can create accounts


### Access Control - Advanced
*   Ability to invite new users 
*   Ability to have allowed list of Tier 2 users
*   Ability to upgrade Tier 1 users to Tier 2 or 3
*   Restrictions on Tier 2 and 3 users to ontario.ca email addresses


<table>
    <tr>
        <td></td>
        <td><strong>Level 1</strong></td>
        <td><strong>Level 2</strong></td>
        <td><strong>Level 3</strong></td>
    </tr>
    <tr>
        <td>Enter new data</td>
        <td>Yes - invited </td>
        <td>Yes - invited<br/>Yes - owned</td>
        <td>Yes - invited<br/>Yes - owned</td>
    </tr>
    <tr>
        <td>Edit data</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>View data</td>
        <td>No</td>
        <td>Yes - all</td>
        <td>Yes - all</td>
    </tr>
    <tr>
        <td>Archive data</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>Create new data set</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>Edit data set</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>Duplicate data set</td>
        <td>No</td>
        <td>Yes - all</td>
        <td>Yes - all</td>
    </tr>
    <tr>
        <td>View data set</td>
        <td>No</td>
        <td>Yes - all</td>
        <td>Yes - all</td>
    </tr>
    <tr>
        <td>Archive data set</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>Invite users to enter data</td>
        <td>No</td>
        <td>Yes - owned</td>
        <td>Yes - owned</td>
    </tr>
    <tr>
        <td>Export data</td>
        <td>No</td>
        <td>Yes - all</td>
        <td>Yes - all</td>
    </tr>
    <tr>
        <td>Search data</td>
        <td>No</td>
        <td>Yes - all</td>
        <td>Yes - all</td>
    </tr>
</table>

