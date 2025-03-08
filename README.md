fardeenkhan
# myfirstgithub.repo
package com.jpmc.midascore.repository;

import com.jpmc.midascore.entity.UserRecord;
import org.springframework.data.repository.CrudRepository;
import java.util.Optional;

public interface UserRepository extends CrudRepository<UserRecord, Long> {
    Optional<UserRecord> findById(Long id); // Optional is the correct return type
}
