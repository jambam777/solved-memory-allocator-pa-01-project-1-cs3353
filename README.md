Download Link: https://assignmentchef.com/product/solved-memory-allocator-pa-01-project-1-cs3353
<br>
<span style="font-size: 2em;">Project Description</span>

<p dir="auto">Implement a custom memory manager in C++ that compares the performance/efficiency of three different allocation strategies/algorithms:

<ol dir="auto">

 <li><strong>Best Fit</strong> – The allocator chooses the smallest area of memory that is available that is large enough for the desired allocation.</li>

 <li><strong>First Fit</strong> – The allocator chooses the first area of memory that is of sufficient size for the desired allocation</li>

 <li><strong>Custom Designed</strong> – The algorithm chooses a location for the allocation based on a scheme you design yourself.</li>

</ol>

<p dir="auto">The custom allocator should overload the <code>new</code>, <code>new[]</code>, <code>delete</code>, <code>delete[]</code> operators as well as any other versions of those operators you see fit. They should be overloaded at the global scope.

<p dir="auto">The allocation and de-allocation operators should make use of a custom Allocator class whose functionality is exposed through an <code>AllocatorSingleton</code> object using the <a href="https://en.wikipedia.org/wiki/Singleton_pattern" rel="nofollow">Singleton Design Pattern</a>. The implementation of each allocation strategy should be through a subclass of Allocator. Implementing the relationship between the allocator and its subclasses should be done using the <a href="https://en.wikipedia.org/wiki/Strategy_pattern" rel="nofollow">Strategy Design Pattern</a>. Note: Allocator and AllocatorSingleton are different classes.

<h3 dir="auto"><a id="user-content-stress-testing-your-implementation" class="anchor" href="https://github.com/smu-cs-3353/project_docs/blob/master/proj01.md#stress-testing-your-implementation" aria-hidden="true"></a>Stress Testing your Implementation</h3>

<p dir="auto">You’ll design and implement two versions of stress testing:

<ol dir="auto">

 <li><p dir="auto">Artificial Testing – Designing a strategy of generating allocation sets of increasing size and complexity solely for the purpose of testing allocations. Example of one data set: randomly generate allocation sizes between 4 and 1024 bytes. Devise a way to randomly allocate and de-allocate (intermingled) chunks of memory for each of those sizes. Based on your knowledge of machine organization, memory management, etc., you are encouraged to devise at least four different experiments you will carry out.</li>

 <li><p dir="auto">Real World Testing – How does your memory allocator perform when used in either the Sentiment Analysis project or Search Engine from 2341? Test it with increasingly large data sets.</li>

</ol>

<p dir="auto">Your stress testing strategies should include your peer group’s minimal. You’ll compare and contrast the performance of your implementation with that of your peers in week of the project.

<h2 dir="auto"><a id="user-content-deliverables" class="anchor" href="https://github.com/smu-cs-3353/project_docs/blob/master/proj01.md#deliverables" aria-hidden="true"></a>Deliverables</h2>

<h3 dir="auto"><a id="user-content-implementation" class="anchor" href="https://github.com/smu-cs-3353/project_docs/blob/master/proj01.md#implementation" aria-hidden="true"></a>Implementation</h3>

<ul dir="auto">

 <li>You should submit a complete implementation of your memory manager along with the relevant stress testing code.</li>

 <li>Your code base should adhere to the following standards and guiding principles:

  <ol dir="auto">

   <li>To the extent possible, your code should be self documenting.</li>

   <li>Use code documentation (comments) where needed to contextualize or otherwise explain challenging or dense blocks of code.</li>

   <li>Your code should build without warnings when using the <code>-Wall</code> flag with g++.</li>

   <li>A full and complete guide to running your project in the spirit or “Reproducible Research”</li>

  </ol></li>

</ul>

<h3 dir="auto"><a id="user-content-analysis-paper" class="anchor" href="https://github.com/smu-cs-3353/project_docs/blob/master/proj01.md#analysis-paper" aria-hidden="true"></a>Analysis Paper</h3>

<p dir="auto">Compose an analysis paper to include the following:

<ul dir="auto">

 <li>An introduction to the project in your own words. Include any hypotheses you have regarding the performance of the various strategies in different allocation environments or conditions.</li>

 <li>An explanation of your specific implementation of the three placement strategies. You may include pseudocode to help your explanation, but no code can be included.</li>

 <li>A detailed methodology of how you stress-tested your allocator and various strategies. This should be in sufficient detail that another student in the class or Dr. Fontenot could reproduce your testing methodology absent your actual source code.</li>

 <li>Describe the results of your tests. To the extent possible, use proper mathematical and statistical strategies for characterizing the data you collected. Graphs and tables are appropriate for this section. Note that this should communicate what data was collected, but not veer into the analysis of the results.</li>

 <li>In narrative form, provide an analysis of results of the experiments. Other graphs and tables may be needed or you may refer to tables or graphs from results description.</li>

</ul>