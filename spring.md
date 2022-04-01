java 
------------------

@Override
//오버라이드

@Enumerated(EnumType.STRING)

메소드

ToStringBuilder
//객체마다 기본적으로 포함된 toString 에 대해서 자동으로 모든 변수들의 이름을
//포함하여, toString 을 만들어준다. (형식도 선택할 수 있음.)
//이젠 멤버 변수를 추가 하더라도 .toString() 메소드에서 누락되는 일은 없을겁니다.
@Override
public String toString() {
  return ToStringBuilder.reflectionToString(this, ToStringStyle.JSON_STYLE);
}

------------------
spring

@SpringBootApplication

@Configuration

@Bean

@ComponentScan

@EnableAspectJAutoProxy

@EnableScheduling

@Validated

@EnableHypermediaSupport(type = EnableHypermediaSupport.HypermediaType.HAL)

@Autowired
//IOC contatiner에 싱글턴으로 사용할 수 있게 넣어줌.

@RestController
//rest api mapping 시 사용

@RequestMapping
//url mapping 시 사용

@Synchronized

@Transactional

@GetMapping

@PostMapping

@LogPrivacyAccess
//lemoncare
@LogAdminExecution
//lemoncare

@PutMapping
----------------
lombok

@Slf4j
//log관련

@Getter

@Setter

@Data

-----------------
validation

@NotBlank
//null과 ""와 " "(빈공백문자열)를 허용하지 않음.

@NotEmpty
//null과 ""를 허용하지 않음.

@NotNull
//모든 데이터 타입에 대해 null을 허용하지 않음.

@Pattern
//값이 정규표현식에 일치하는지 검사

@AssertTure
//true인지 검사

@AssertFalse
//false인지 검사

@JsonProperty
