
### Most used Spring Annotations 

 - @Component : Indicates a spring bean
 - @Controller : Indicates a controller component
 - @Service : Indicates a Model component
 - @Repository : Indicates a DAO component used to perform CURD/CRUD operations
 - @Required : Indicates a mandatory bean configuration for specified property. Container throws BeanInitializationException it is not found.
 - @Autowired : Container finds specified bean byType
 - @Qualifier : Used in conjunction with @Autowired. Container finds specified bean byName
 - @Scope : by default it is singleton.
   - singleton : single instance
   - prototype : creates a new bean instance of the object every time a request for that specific bean is made. As a rule, use the prototype scope for all state-full beans and the singleton scope for stateless beans.
   - request : This scopes a bean definition to an HTTP request. Only valid in the context of a web-aware Spring ApplicationContext.
   - session : This scopes a bean definition to an HTTP session. Only valid in the context of a web-aware Spring ApplicationContext.
   - global-session : This scopes a bean definition to a global HTTP session. Only valid in the context of a web-aware Spring ApplicationContext.
 

### Java Based Configuration

@Configuration
@ComponentScan
@Import
@DependsOn
@Bean
@Lazy
@Value

@Transactional
- PropagationType
- IsolationLevel
- timeout
- read-only 

@EnableAutoConfiguration
@SpringBootApplication

@RestController
@RequestMapping
@GetMapping
@PostMapping
@PutMapping
@PatchMapping
@DeleteMapping

@PathVariable
@RequestAttribute
@RequestParam
@RequestBody
@RequestHeader
@RequestPart

@ResponseBody
@ResponseStatus

@ModelAttribute

@PreAuthorize

@SessionAttribute
@SessionAttributes

### Cache related Annotations
@Cacheable
@CachePut
@CacheEvict
@CacheConfig

### Task Execution and Scheduling Annotations
@Scheduled
@Async

#### Testing related Annotations
@BootstrapWith
@ContextConfiguration
@WebAppConfiguration
@Timed
@Repeat




@ExceptionHandler

