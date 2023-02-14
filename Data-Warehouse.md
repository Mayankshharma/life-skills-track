# What is Data Ware House?

A data warehouse is a central repository of information that can be analyzed to make more informed decisions. Data flows into a data warehouse from transactional systems, relational databases, and other sources, typically on a regular cadence. Business analysts, data engineers,  data scientists, and decision-makers access the data through business intelligence (BI) tools, SQL clients, and other analytics applications.

# What are the benefits of using a data warehouse?
The benefits of a data warehouse include the following:

* Informed decision making
* Consolidated data from many sources
* Historical data analysis
* Data quality, consistency, and accuracy
* Separation of analytics processing from transactional databases, which improves the performance of both systems

# Data Warehouse Architecture
Usually, data warehouse architecture comprises a three-tier structure.

* Bottom Tier
The bottom tier or data warehouse server usually represents a relational database system. Back-end tools are used to cleanse, transform and feed data into this layer. 

* Middle Tier
The middle tier represents an OLAP server that can be implemented in two ways. 

   The ROLAP or Relational OLAP model is an extended relational database management system that maps multidimensional data processes to standard relational processes. 

  The MOLAP or multidimensional OLAP directly acts on multidimensional data and operations.

* Top Tier
This is the front-end client interface that gets data out from the data warehouse. It holds various tools like query tools, analysis tools, reporting tools, and data mining tools

# How Data Warehouse Works
Data Warehousing integrates data and information collected from various sources into one comprehensive database. For example, a data warehouse might combine customer information from an organization’s point-of-sale systems, its mailing lists, website, and comment cards. It might also incorporate confidential information about employees, salary information, etc. Businesses use such components of the data warehouse to analyze customers. 

Data mining is one of the features of a data warehouse that involves looking for meaningful data patterns in vast volumes of data and devising innovative strategies for increased sales and profits. 

# Some Example Code 

st.title('Dashboard')
column_1, column_2 = st.beta_columns(2)

with column_1:
    st.header('Save records')
    name = st.text_input('Please enter name')
    details = st.text_input('Please enter details (separated by comma)')
    details = ('{%s}' % (details))
    if st.button('Save record to database'):
        write_record(name,details,engine)
        st.info('Name: **%s** and details: **%s** saved to database' % (name,details[1:-1]))


# Reference link

* [Aws](https://aws.amazon.com/data-warehouse/#:~:text=A%20data%20warehouse%20is%20a,typically%20on%20a%20regular%20cadence.) 

* [Medium](https://towardsdatascience.com/building-a-data-warehouse-in-python-using-postgresql-f10dce22e3aa)

* [Simplilearn](https://www.simplilearn.com/data-warehouse-article)
